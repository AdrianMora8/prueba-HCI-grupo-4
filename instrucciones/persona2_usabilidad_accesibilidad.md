# Integrante 2 — Usabilidad y Accesibilidad + Pantalla "Docente y horario"

> **Instrucciones para IA:** si vas a usar un asistente de IA, pégale este archivo
> completo junto con `00_contexto_comun.md`. Pídele que te ayude a definir metas
> NUMÉRICAS y realistas para los indicadores (no dejar "Definir meta" en blanco),
> basadas solo en E2, E3, E4, E6 y E9. No debe inventar datos que no estén en el caso.

Lee primero `00_contexto_comun.md` (caso, evidencias, estándar visual, reglas de GitHub).

## Tu entregable de análisis 1: Indicadores de usabilidad

Completa la tabla con indicador Y meta numérica (no dejes "Definir meta" literal):

| Dimensión | Indicador y forma de medir | Meta (tú la defines, con lógica) |
|---|---|---|
| Efectividad | % de participantes que completan la reserva sin ayuda | Ej: ≥ 90% (basado en que el proceso actual ya funciona pero es lento, E4) |
| Eficiencia | Tiempo y cantidad de acciones para reservar | Ej: ≤ 2 minutos y máximo 5 toques (contra los 14 min / 9 mensajes actuales, E4) |
| Satisfacción | Valoración post-tarea en escala 1 a 7 | Ej: promedio ≥ 6 |
| Aprendizaje o errores | Primer intento, errores observados, recuperación | Ej: 0 selecciones de horarios ocupados en primer intento (contra los 3 casos de E3) |

## Tu entregable de análisis 2: Decisiones POUR (accesibilidad)

| Principio | Decisión que aplicarás | Cómo se verifica |
|---|---|---|
| Perceptible | Texto, contraste y comunicación de estados sin depender solo del color | Inspección visual de pantallas (revisa que el estado "ocupado" tenga texto/ícono, no solo rojo) — usa E9 |
| Operable | Orden de teclado, foco visible, controles accionables | Recorre la pantalla 2 solo con Tab/Enter, sin mouse — usa E2 |
| Comprensible | Etiquetas claras, consistencia, mensajes que expliquen cómo corregir un error | Simula el error "horario ya ocupado" y revisa que el mensaje diga qué hacer — usa E3 |
| Robusto | Estructura y nombres interpretables por lector de pantalla | Revisa que cada elemento tenga una etiqueta de texto real (no solo ícono) — usa E2 |

**Dónde lo guardas:** `docs/02_usabilidad_accesibilidad.pdf` (exporta ambas tablas desde FigJam).

## Tu pantalla: "2. Docente y horario"

**Contenido mínimo obligatorio:**
- Disponibilidad por fecha (un calendario o lista de fechas).
- Horarios diferenciados visualmente en 3 estados: **disponible**, **ocupado**, **seleccionado** (usa las tarjetas de horario del estándar visual, con texto además de color).

**Conceptos que debes evidenciar:**
- **Calendario (metáfora):** reconocible sin explicación (E9).
- **Affordance y mapeo:** un horario disponible debe *parecer* seleccionable (borde, sombra, cursor), uno ocupado debe *parecer* bloqueado.
- **Teclado:** todos los horarios deben poder recorrerse con Tab y seleccionarse con Enter/Espacio — dilo explícitamente en tu documentación aunque el prototipo sea estático.
- **Prevención de errores:** un horario ocupado NO debe poder seleccionarse (contra los 3 intentos fallidos de E3).

**Evidencia a citar:** E2 (teclado, zoom 200%, lector de pantalla), E3 (intentos de seleccionar horarios ocupados), E6 (disponibilidad depende del docente), E9 (reconocimiento del calendario).

## Checklist antes de dar por terminada tu parte

- [ ] Los 4 indicadores tienen meta numérica, ninguno dice "Definir meta".
- [ ] Las 4 decisiones POUR son verificables en tu pantalla (no solo teóricas).
- [ ] Pantalla 2 muestra los 3 estados de horario con texto/ícono, no solo color.
- [ ] Exportaste `docs/02_usabilidad_accesibilidad.pdf`.
- [ ] Exportaste la captura de tu pantalla a `prototipo/capturas/`.

## Pasos exactos en GitHub

1. Crea el issue: **"Usabilidad y accesibilidad: indicadores + POUR + pantalla Horario"**, descripción: "Definir 3 indicadores con meta, 4 decisiones POUR, y construir pantalla 2 Docente y horario con estados diferenciados."
2. Crea la rama: `feature/usabilidad-accesibilidad`.
3. Commit 1 (ejemplo): `Agrega indicadores de usabilidad con metas basadas en E3 y E4`.
4. Commit 2 (ejemplo): `Agrega pantalla Docente y horario con estados disponible, ocupado y seleccionado`.
5. Abre el PR, título: "Usabilidad/Accesibilidad + Pantalla Horario", vincula el issue (`Closes #N`).
6. Pide revisión a otro integrante distinto al que revisa tu propio issue.
