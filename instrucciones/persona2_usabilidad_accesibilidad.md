# Integrante 2 — Usabilidad y Accesibilidad (análisis, sin Figma)

> **Instrucciones para IA:** si vas a usar un asistente de IA, pégale este archivo
> completo junto con `00_contexto_comun.md`. Pídele que te ayude a definir metas
> NUMÉRICAS y realistas para los indicadores (no dejar "Definir meta" en blanco),
> basadas solo en E2, E3, E4, E6 y E9. Tu resultado final debe ser lo bastante
> específico para que OTRA persona, sin hablar contigo, pueda construir la pantalla
> correcta en Figma solo leyendo tu documento.

Lee primero `00_contexto_comun.md` (caso, evidencias, estándar visual, reglas de GitHub, y cómo está dividido el trabajo).

**Tu issue:** [#2](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/2) — asignado a Sebasjach21.

**Importante:** tú NO construyes ninguna pantalla. Tu trabajo es análisis + dejar
especificaciones tan claras que la persona 4 (quien construye el prototipo completo)
pueda implementarlas sin preguntarte nada.

## Parte A — Indicadores de usabilidad

Completa la tabla con indicador Y meta numérica (no dejes "Definir meta" literal):

| Dimensión | Indicador y forma de medir | Meta (tú la defines, con lógica) |
|---|---|---|
| Efectividad | % de participantes que completan la reserva sin ayuda | Ej: ≥ 90% (basado en que el proceso actual ya funciona pero es lento, E4) |
| Eficiencia | Tiempo y cantidad de acciones para reservar | Ej: ≤ 2 minutos y máximo 5 toques (contra los 14 min / 9 mensajes actuales, E4) |
| Satisfacción | Valoración post-tarea en escala 1 a 7 | Ej: promedio ≥ 6 |
| Aprendizaje o errores | Primer intento, errores observados, recuperación | Ej: 0 selecciones de horarios ocupados en primer intento (contra los 3 casos de E3) |

## Parte B — Decisiones POUR (accesibilidad)

| Principio | Decisión que aplicarás | Cómo se verifica |
|---|---|---|
| Perceptible | Texto, contraste y comunicación de estados sin depender solo del color | Inspección visual de pantallas (revisa que el estado "ocupado" tenga texto/ícono, no solo rojo) — usa E9 |
| Operable | Orden de teclado, foco visible, controles accionables | Recorre la pantalla 2 solo con Tab/Enter, sin mouse — usa E2 |
| Comprensible | Etiquetas claras, consistencia, mensajes que expliquen cómo corregir un error | Simula el error "horario ya ocupado" y revisa que el mensaje diga qué hacer — usa E3 |
| Robusto | Estructura y nombres interpretables por lector de pantalla | Revisa que cada elemento tenga una etiqueta de texto real (no solo ícono) — usa E2 |

## Especificaciones para el prototipo (esto es lo que persona 4 va a implementar)

Escribe una lista de instrucciones concretas, dirigidas a quien construye,
indicando en qué pantalla aplica cada decisión POUR (usa la tabla de las 4
pantallas en `00_contexto_comun.md`). Cubre obligatoriamente:

- Qué texto/ícono exacto debe acompañar cada estado de color (disponible/ocupado/
  seleccionado/confirmado/error) para cumplir "Perceptible".
- El orden de tabulación (Tab) esperado en la Pantalla 2 (Docente y horario) para
  cumplir "Operable" — descríbelo como una secuencia numerada.
- El texto exacto del mensaje de error cuando alguien intenta seleccionar un
  horario ocupado, para cumplir "Comprensible" (referencia E3).
- Qué etiquetas de texto (no solo íconos) debe llevar cada componente interactivo,
  para cumplir "Robusto" (referencia E2).

**Dónde lo guardas:** `docs/02_usabilidad_accesibilidad.pdf` (ambas tablas +
especificaciones para el prototipo).

## Checklist antes de dar por terminada tu parte

- [ ] Los 4 indicadores tienen meta numérica, ninguno dice "Definir meta".
- [ ] Las 4 decisiones POUR son verificables, no solo teóricas.
- [ ] Especificaciones por pantalla redactadas (textos exactos, orden de teclado,
      mensajes de error) para que persona 4 no tenga que inventar nada.
- [ ] Exportaste `docs/02_usabilidad_accesibilidad.pdf`.

## Pasos exactos en GitHub

1. El issue ya existe: [#2](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/2) "Usabilidad y accesibilidad".
2. Crea tu propia rama: `feature/usabilidad-accesibilidad` (desde `main`, créala tú).
3. Commit 1 (ejemplo): `Agrega indicadores de usabilidad con metas basadas en E3 y E4`.
4. Commit 2 (ejemplo): `Agrega decisiones POUR y especificaciones de accesibilidad para el prototipo`.
5. Abre el PR, título: "Usabilidad y accesibilidad", vincula el issue (`Closes #2`).
6. Pide revisión a otro integrante distinto al que revisa tu propio issue.
