# Integrante 4 — Construcción completa del prototipo (Figma/Penpot) + guía de estilo + prueba cruzada

> **Instrucciones para IA:** si vas a usar un asistente de IA, pégale este archivo
> completo junto con `00_contexto_comun.md`. Úsala para revisar que no te falte
> ningún elemento obligatorio por pantalla, no para inventar contenido: el
> contenido real de cada pantalla sale de los documentos de las personas 1, 2 y 3
> en `docs/` (léelos antes de construir).

Lee primero `00_contexto_comun.md` (caso, evidencias, estándar visual, reglas de GitHub, y cómo está dividido el trabajo).

**Tu issue:** [#4](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/4) — asignado a MatiusJBG.

**Importante:** tú eres el único integrante que abre Figma/Penpot. Antes de
construir, lee los 3 documentos que las otras personas suben a `docs/`:
- `docs/01_matriz_ihc.pdf` y `docs/04_decisiones_diseno.pdf` (persona 1): metáfora, affordance, Gestalt, carga cognitiva — con especificaciones por pantalla.
- `docs/02_usabilidad_accesibilidad.pdf` (persona 2): textos de estado, orden de teclado, mensajes de error.
- `docs/03_dcu_contexto.pdf` (persona 3): qué debe contener cada pantalla según los 5 requisitos.

Si algún documento aún no está subido cuando quieras avanzar, empieza por la guía
de estilo y la estructura de las pantallas (abajo) — no tienes que esperar a los 3
al mismo tiempo, puedes ir incorporando cada documento a medida que llega.

## Paso 1 — Guía de estilo (defínela primero, antes de dibujar nada)

| Elemento | Definición |
|---|---|
| Tipografía | Título 20px bold · Subtítulo 16px semibold · Cuerpo 14px regular · Auxiliar 12px regular gris `#6B6B6B` |
| Color | Acción principal `#2F6FED` · Fondo `#FFFFFF` · Texto `#1A1A1A` · Éxito `#1E9E5A` (+ ícono ✓ + texto) · Error `#D93636` (+ ícono ✕ + texto) |
| Componentes | Botón primario/secundario, campo de texto (normal/foco/error), tarjeta de horario (disponible/ocupado/seleccionado), tarjeta de tutoría, mensaje de estado |
| Consistencia | Mismas etiquetas, misma ubicación de acciones, misma respuesta del sistema en las 4 pantallas |

Crea estos componentes **una sola vez** en una página "🎨 Componentes" de tu archivo
y reutilízalos como instancias en las 4 pantallas — no los redibujes por pantalla.

## Paso 2 — Construir las 4 pantallas conectadas

| # | Pantalla | Contenido mínimo obligatorio | Conceptos que deben verse |
|---|---|---|---|
| 1 | Inicio y búsqueda | Objetivo claro, acceso a "Reservar" y a "Mis tutorías" | Jerarquía, figura-fondo, consistencia, navegación |
| 2 | Docente y horario | Disponibilidad por fecha; horario seleccionado y ocupado diferenciados (texto/ícono, no solo color) | Calendario, affordance, mapeo, teclado, prevención de errores |
| 3 | Resumen y confirmación | Docente, fecha, hora, modalidad, acción "Confirmar", opción "Volver" | Reconocimiento, carga cognitiva, retroalimentación, corrección |
| 4 | Confirmada y reprogramación | Estado inequívoco de "Confirmado", datos de la cita, entrada al cambio de horario | Visibilidad del estado, recuperación, manipulación directa |

Para cada pantalla, aplica literalmente las especificaciones que dejaron las
personas 1, 2 y 3 en sus PDFs (metáforas, textos de error exactos, orden de
teclado, contenido derivado de los requisitos). No decidas contenido nuevo por tu
cuenta si ya está especificado — tu trabajo es construir fielmente lo analizado,
no reinterpretarlo.

Conecta las 4 pantallas con **Prototype mode** (flechas de navegación) para que el
recorrido completo (reservar → confirmar → ver confirmación → reprogramar) se
pueda ejecutar sin explicación verbal.

## Paso 3 — Prueba cruzada e iteración

1. Entrega el prototipo YA CONECTADO a una persona de otro equipo, sin explicarle cómo funciona.
2. Pídele: "reserva una tutoría para el jueves y luego cambia el horario".
3. Registra: si completó la tarea, tiempo aproximado, error o duda observable, comentario final.
4. Aplica una mejora concreta relacionada con el hallazgo (guarda captura antes/después).
5. Documenta todo en `evaluacion/prueba_iteracion.md` (tarea, participante, resultado, tiempo, hallazgo, antes, después).
6. Haz el commit de esa mejora vinculado al issue/PR correspondiente.

## Checklist antes de dar por terminada tu parte

- [ ] Archivo de Figma/Penpot creado, con página "🎨 Componentes" reutilizada en las 4 pantallas.
- [ ] Las 4 pantallas cumplen su contenido mínimo obligatorio de la tabla de arriba.
- [ ] Incorporaste las especificaciones de las personas 1, 2 y 3 (no inventaste contenido nuevo).
- [ ] Las 4 pantallas están conectadas y navegables en Prototype mode.
- [ ] Prueba cruzada ejecutada y documentada en `evaluacion/prueba_iteracion.md`.
- [ ] Enlace del archivo pegado en `prototipo/enlace_prototipo.md`, verificado en ventana privada.
- [ ] Capturas de las 4 pantallas en `prototipo/capturas/`.

## Pasos exactos en GitHub

1. El issue ya existe: [#4](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/4) "Construir el prototipo completo + guía de estilo + prueba cruzada e iteración".
2. Crea tu propia rama: `feature/prototipo-completo` (desde `main`, créala tú).
3. Commit 1 (ejemplo): `Agrega guia de estilo y sistema de componentes reutilizables`.
4. Commit 2 (ejemplo): `Agrega las 4 pantallas conectadas del prototipo`.
5. Commit 3 (ejemplo, cuando esté lista): `Agrega hallazgo y mejora de la prueba cruzada`.
6. Abre el PR, título: "Prototipo completo + guía de estilo + prueba cruzada", vincula el issue (`Closes #4`).
7. Pide revisión a otro integrante.
