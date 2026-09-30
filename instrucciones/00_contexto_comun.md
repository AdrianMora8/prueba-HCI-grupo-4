# Contexto común del caso — leer antes de tu tarea individual

> Este bloque es el mismo para los 4 integrantes. Está aquí para que, si usas una IA
> para ayudarte, puedas pegar este archivo completo (contexto + tu tarea) y la IA
> tenga todo lo necesario sin inventar información fuera del caso.

## Repositorio del equipo

**https://github.com/AdrianMora8/prueba-HCI-grupo-4**

Ya estás agregado como colaborador. Cada quien crea su propia rama `feature/...`
desde `main` cuando empiece a trabajar.

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

## Cómo trabajamos todos en el mismo Figma (un solo enlace para entregar)

Como el prototipo pide **un enlace único** pero cada quien diseña una pantalla
distinta, la forma correcta es usar **UN SOLO archivo de Figma compartido**, no 4
archivos separados:

1. La persona del issue #4 (decisiones de diseño / guía de estilo) crea el archivo
   Figma del equipo y arma primero la página "🎨 Componentes" con el estándar visual.
2. Esa persona comparte el archivo con el resto vía **Share → Invite** usando el
   correo o usuario de Figma de cada integrante (permiso de "Can edit"), o con el
   toggle "Anyone with the link can edit" si prefieren agilizar.
3. Dentro de ESE MISMO archivo, cada integrante crea su propio frame/página con el
   nombre de su pantalla (`01-Inicio`, `02-Horario`, `03-Confirmacion`,
   `04-Confirmada`) y trabaja ahí. Figma es multijugador en tiempo real: todos
   pueden estar editando simultáneamente, como en Google Docs, sin pisarse el
   trabajo si cada quien se queda en su propio frame.
4. Al final, entre todos conectan los 4 frames con **Prototype mode** (flechas de
   navegación entre pantallas).
5. Se copia **un solo enlace** de ese archivo (modo presentación o el link del
   archivo con permiso de vista) y se pega en `prototipo/enlace_prototipo.md`. Ese
   es el enlace que se entrega en Moodle — no hay que combinar ni exportar nada de
   4 archivos distintos porque nunca existieron 4 archivos.
6. Cada quien exporta la captura de SU pantalla desde ese archivo compartido y la
   sube a `prototipo/capturas/` en su propio commit.

## Reglas de GitHub que aplican a TODOS

- 1 issue asignado a ti, con objetivo y producto esperado claro.
- 1 rama propia `feature/tu-aporte`.
- Mínimo **2 commits sustanciales** (no triviales, no "actualización", deben describir
  el cambio real).
- 1 Pull Request propio, con descripción y el issue relacionado.
- Revisar el PR de **otro** compañero (no el tuyo).
- Nunca trabajar directo en `main`.
