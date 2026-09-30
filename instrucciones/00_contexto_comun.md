# Contexto común del caso — leer antes de tu tarea individual

> Este bloque es el mismo para los 4 integrantes. Está aquí para que, si usas una IA
> para ayudarte, puedas pegar este archivo completo (contexto + tu tarea) y la IA
> tenga todo lo necesario sin inventar información fuera del caso.

## Repositorio del equipo

**https://github.com/AdrianMora8/prueba-HCI-grupo-4**

Ya estás agregado como colaborador. Cada quien crea su propia rama `feature/...`
desde `main` cuando empiece a trabajar (las ramas ya NO vienen pre-creadas).

## Cómo está dividido el trabajo (una sola persona construye el prototipo)

Para que nadie dependa de otro mientras trabaja, y para que el prototipo sea
visualmente consistente sin tener que coordinar edición simultánea en Figma, el
equipo se organiza así:

- **Personas 1, 2 y 3 (análisis):** cada una investiga su tema y entrega un
  **documento con especificaciones exactas** de qué debe aparecer en cuál pantalla
  y por qué (citando evidencia E1–E10). No tocan Figma. Su commit son PDFs/markdown
  en `docs/`.
- **Persona 4 (prototipo):** es la única que abre Figma. Toma las especificaciones
  de las otras 3 personas (ya publicadas en sus PDFs dentro de `docs/`, disponibles
  para todos en el repo) y construye las 4 pantallas conectadas, aplicando también
  la guía de estilo. Esto evita conflictos de edición y da un solo archivo, un solo
  enlace, un solo estilo consistente.

**Por qué nadie depende de nadie en tiempo real:** las personas 1, 2 y 3 trabajan en
paralelo desde el inicio (todas parten de las mismas evidencias E1–E10, no del
resultado de otra). Solo publican sus especificaciones (commit + push) para que la
persona 4 las lea cuando le toque construir cada pantalla — no necesitan estar
conectados al mismo tiempo ni coordinar en vivo.

**Entrega del enlace:** la persona 4 crea el archivo de Figma/Penpot, construye las
4 pantallas con **Prototype mode** conectándolas, y copia el enlace (modo
presentación o vista) en `prototipo/enlace_prototipo.md`. Ese es el único enlace
que se entrega en Moodle.

## El reto

Diseñar desde cero **"Tutoría Fácil UTA"**, una app web móvil que permita **consultar
disponibilidad, reservar, confirmar y reprogramar** una tutoría académica. No existe
interfaz previa; solo el proceso actual (manual) y las evidencias de abajo.

## Proceso actual (lo que hay que reemplazar)

La Facultad coordina tutorías por WhatsApp, hojas de cálculo y agendas personales.
El estudiante escribe al docente, espera respuesta, propone horarios y pide
confirmación. Si necesita cambiar la cita, empieza otra conversación. No hay sistema
interactivo unificado.

## Problema de diseño

¿Cómo permitir que un estudiante reserve o reprograme una tutoría desde un teléfono,
con claridad, bajo esfuerzo cognitivo, prevención de errores y acceso mediante
teclado o tecnologías de apoyo?

## Alcance (qué SÍ y qué NO diseñar)

- Empieza cuando el estudiante busca un horario, termina cuando obtiene una
  confirmación comprensible.
- Debe incluir una ruta para **reprogramar** una cita existente.
- **NO** se diseña: autenticación (login), reportes, ni administración de usuarios.

## Evidencias del caso (E1–E10) — cita siempre al menos una en cada decisión

| ID | Evidencia |
|----|-----------|
| E1 | Laura, 20 años, revisa horarios desde el teléfono viajando en bus. Necesita reservar sin intercambiar varios mensajes. |
| E2 | Carlos usa teclado, ampliación al 200% y lector de pantalla. Los calendarios sin etiquetas son difíciles de comprender. |
| E3 | Observación de 12 solicitudes: 4 confirmaciones ambiguas y 3 intentos de seleccionar horarios ya ocupados. |
| E4 | Tiempo medio del proceso actual: 14 minutos y 9 mensajes hasta confirmar. |
| E5 | Dos estudiantes olvidaron la fecha acordada porque la confirmación se mezcló con otros mensajes. |
| E6 | Los docentes reciben solicitudes fuera de horario y actualizan su disponibilidad manualmente. |
| E7 | La secretaria transcribe cambios a una hoja de cálculo y puede tener información desactualizada. |
| E8 | La conexión móvil es variable; las acciones principales deben ser comprensibles si una respuesta tarda. |
| E9 | Los estudiantes reconocen calendario, tarjeta de cita y estado confirmado, pero no todos interpretan íconos aislados. |
| E10 | Los usuarios esperan poder deshacer o corregir una selección antes de confirmar definitivamente. |

## Las 4 pantallas del prototipo (visión completa del flujo)

| # | Pantalla | Contenido mínimo | Conceptos que deben verse |
|---|----------|-------------------|----------------------------|
| 1 | Inicio y búsqueda | Objetivo claro, acceso a reservar y a mis tutorías | Jerarquía, figura-fondo, consistencia, navegación |
| 2 | Docente y horario | Disponibilidad por fecha; horario seleccionado y ocupado diferenciados | Calendario, affordance, mapeo, teclado, prevención de errores |
| 3 | Resumen y confirmación | Docente, fecha, hora, modalidad, acción confirmar, opción volver | Reconocimiento, carga cognitiva, retroalimentación, corrección |
| 4 | Confirmada y reprogramación | Estado inequívoco, datos de la cita, entrada al cambio de horario | Visibilidad del estado, recuperación, manipulación directa |

## Estándar visual obligatorio (síguelo en tu pantalla, no inventes otro estilo)

**Colores**
- Acción principal: `#2F6FED`
- Fondo: `#FFFFFF`
- Texto: `#1A1A1A`
- Éxito/confirmado: `#1E9E5A` + ícono ✓ + palabra "Confirmado" (nunca solo color)
- Error/ocupado: `#D93636` + ícono ✕ + palabra "No disponible" (nunca solo color)

**Tipografía** (una sola familia, ej. Inter/Roboto)
- Título: 20px bold · Subtítulo: 16px semibold · Cuerpo: 14px regular · Auxiliar: 12px regular gris `#6B6B6B`

**Espaciado**: grid de 8px (8/16/24/32), márgenes laterales 16px.

**Componentes reutilizables (usa instancias de Figma, no los redibujes)**
Botón primario/secundario · Campo de texto (normal/foco/error) · Tarjeta de horario
(disponible/ocupado/seleccionado) · Tarjeta de tutoría · Mensaje de estado.

## Reglas de GitHub que aplican a TODOS

- 1 issue asignado a ti, con objetivo y producto esperado claro.
- 1 rama propia `feature/tu-aporte`.
- Mínimo **2 commits sustanciales** (no triviales, no "actualización", deben describir
  el cambio real).
- 1 Pull Request propio, con descripción y el issue relacionado.
- Revisar el PR de **otro** compañero (no el tuyo).
- Nunca trabajar directo en `main`.
