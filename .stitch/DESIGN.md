---
version: alpha
name: Bei Treino
description: Baseline visual y dirección de rediseño premium para iPhone y Apple Watch
colors:
  primary: "#132A35"
  accent: "#C5EE64"
  surface: "#F7F8F4"
  secondary: "#54DACA"
  warning: "#FF785A"
  recovery: "#8267D5"
  success: "#197361"
  error: "#B5473D"
typography:
  headline-display:
    fontFamily: Manrope
    fontSize: 44px
    fontWeight: 800
    lineHeight: 1.05
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Manrope
    fontSize: 34px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.2
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Manrope
    fontSize: 17px
    fontWeight: 600
    lineHeight: 1.2
rounded:
  sm: 12px
  md: 16px
  lg: 20px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
  xxl: 32px
  screen-margin: 24px
components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    height: 56px
  card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.md}"
    padding: 16px
  workout-card:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: 20px
---

# Bei Treino Design System

## Overview

### Creative North Star

**Un entrenador personal silencioso:** premium, claro y humano; acompaña sin abrumar. La persona debe entender en segundos qué toca hoy, qué acción sigue y qué progreso hizo. El producto no tiene que parecer un panel administrativo ni una web metida en un teléfono.

El iPhone necesita una reconstrucción visual importante. El Watch es el baseline mejor resuelto: fondo oscuro, una tarea por pantalla, información esencial, acción grande y navegación lateral.

### Principles

1. **Una intención principal por pantalla.** El CTA dominante debe ser obvio sin competir con cinco tarjetas.
2. **La rutina es protagonista.** Métricas secundarias acompañan; no desplazan el entrenamiento.
3. **Progreso comprensible, no analítico.** Gráficos breves, comparaciones simples y lenguaje no competitivo.
4. **Premium por edición.** Menos elementos, mejor espaciados; no sumar adornos para generar jerarquía.
5. **Humano y responsable.** Motivación breve, sin culpa y sin afirmaciones médicas.

## Colors

### Core

- Azul Bei: `#132A35` — identidad, superficies oscuras, texto principal.
- Lima Bei: `#C5EE64` — acción primaria, progreso y foco.
- Papel: `#F7F8F4` — fondo cálido principal.
- Aqua: `#54DACA` — datos secundarios y movimiento.
- Coral: `#FF785A` — energía o alerta no destructiva.
- Violeta: `#8267D5` — recuperación y descanso.
- Verde: `#197361` — éxito y finalización.
- Rojo: `#B5473D` — error o acción destructiva.

### Usage rules

- Usar lima para una sola acción primaria visible por región.
- Reservar azul oscuro para contraste, navegación y momentos inmersivos.
- No colorear cada tarjeta con un acento distinto; eso fragmenta la experiencia.
- No usar degradados intensos como solución genérica de jerarquía.
- Estados deben comunicarse con color + icono + texto, nunca solo con color.

## Typography

- Familia actual: **Manrope**.
- Títulos: 700–800, pero con escala contenida en iPhone.
- Texto: 400–600, interlineado generoso.
- Eyebrows en mayúsculas: uso excepcional; no deben preceder cada sección.
- Números de entrenamiento y temporizadores: tabular, alto contraste.

Escala recomendada para iPhone:

- Display: 40–44 pt, máximo dos líneas.
- H1: 32–36 pt.
- H2: 22–26 pt.
- Body: 16–18 pt.
- Caption: 13–15 pt.
- CTA: 17–18 pt semibold.

## Layout

- Base: 4 pt; pasos principales: 8, 12, 16, 24, 32.
- Margen de pantalla: 20–24 pt.
- Altura táctil mínima: 44 pt; CTA principal preferido: 52–56 pt.

### iPhone

- Respetar Dynamic Island y safe areas; nunca poner marca ni título detrás del sistema.
- Encabezado compacto: identidad o título, no ambos gigantes.
- Navegación inferior estable y sobria, sin tapar contenido ni crear dos selecciones visuales simultáneas.
- Permitir que Inicio sea una pantalla útil sin scroll: rutina de hoy, estado semanal breve y acceso a actividad.
- Pantallas de entrenamiento pueden ser inmersivas y ocultar la navegación global.

### Watch

- Mantener una acción principal por pantalla.
- Desplazamiento horizontal para información complementaria; evitar listas verticales largas.
- No editar peso ni repeticiones con teclado en el reloj.
- Mostrar ejercicio, dosis planificada, progreso, métricas y check grande.
- Descanso: contador, `+15 s` y `Saltar descanso`; sin círculo de respiración.

## Elevation & Depth

- Usar una sola elevación sutil.
- Priorizar borde, contraste tonal y separación espacial antes que sombras.
- Evitar glow pesado y múltiples niveles de sombra en una misma pantalla.

## Shapes

- Radio de tarjeta: 16–20 pt; evitar usar 24–40 pt en todo.
- Radio de controles: 12–16 pt.
- Pills únicamente para estados, filtros u opciones cortas.
- La geometría debe sentirse precisa y atlética, no inflada ni infantil.

## Components

### Bottom navigation

- Cinco destinos: Rutinas, Agenda, Inicio, Progreso y Perfil.
- Inicio puede tener una presencia ligeramente mayor, pero sin convertir la barra en un bloque que tape contenido.
- Selección: cambio de color, icono relleno o indicador corto; una sola señal dominante.
- Evitar glow pesado, cápsulas enormes y doble estado activo.

### Today workout card

- Nombre de rutina, cantidad de bloques/duración estimada y CTA `Empezar`.
- Puede usar superficie azul Bei.
- No mezclar en la misma tarjeta explicaciones largas, métricas y controles secundarios.

### Routine list

- Día, nombre, resumen de bloques y acción de comenzar.
- Editar es una acción secundaria; eliminar usa icono de papelera con confirmación.
- Bloques y ejercicios se presentan por divulgación progresiva.

### Exercise card

- Nombre, dosis planificada, check y progreso de vuelta.
- En modo simple, ajustes de peso/repeticiones quedan colapsados.
- En modo detallado, la última carga sirve como referencia y los campos pueden editarse.

### Rest

- Temporizador central legible.
- Acciones: `+15 segundos` y `Saltar descanso`.
- No introducir gamificación ni respiración obligatoria durante el descanso.

### Agenda

- Planificación semanal, no un calendario administrativo.
- Cada día debe leerse como planificado, completado, descanso o libre.
- Registrar actividad externa y planificar deben ser accesibles, pero no dominar el viewport.

### Progress

- Resumen semanal en una pantalla: días activos, minutos, sesiones y tendencia.
- Gráficos compactos con contexto; evitar una columna interminable de tarjetas.
- Sueño, pasos y Apple Salud son datos opcionales y deben explicar su fuente.

### Completion and sharing

- Felicitación breve y personalizada.
- Resumen visual apto para compartir en Stories.
- Compartir siempre es explícito; la app nunca publica sola.

## Motion

- Transiciones de 180–260 ms.
- Navegación inferior: desplazamiento corto o morph de indicador, sin rebote excesivo.
- Check: haptic ligero + cambio de estado inmediato.
- Gráficos: entrada discreta; respetar Reduce Motion.

## Accessibility

- Compatible con Dynamic Type y VoiceOver.
- Contraste WCAG AA como mínimo.
- Targets de 44×44 pt o mayores.
- No bloquear selección de texto de forma global si perjudica accesibilidad; impedir zoom accidental sin desactivar el zoom de accesibilidad del sistema.
- Estados y errores con texto accionable.
- Probar modo claro, texto grande y pantallas pequeñas.

## Do's and Don'ts

### Do

- Conservar marca, Manrope, azul y lima.
- Diseñar primero la arquitectura y luego el estilo.
- Usar composición, tipografía y espacio para dar sensación premium.
- Mantener el Watch prácticamente como está.

### Don't

- No copiar literalmente la densidad de las capturas actuales.
- No usar una tarjeta para cada oración.
- No hacer todos los botones gigantes ni todas las superficies redondeadas.
- No esconder contenido detrás de la barra inferior.
- No inventar ejercicios, métricas médicas ni recomendaciones clínicas.
