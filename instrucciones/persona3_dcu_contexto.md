# Integrante 3 — Diseño Centrado en el Usuario (DCU) + Pantalla "Resumen y confirmación"

> **Instrucciones para IA:** si vas a usar un asistente de IA, pégale este archivo
> completo junto con `00_contexto_comun.md`. Pídele ayuda para redactar la persona,
> el escenario y el journey map, pero recuérdale explícitamente: "no inventes una
> biografía extensa, la persona debe representar patrones de E1-E10, no rasgos
> decorativos". Los 5 requisitos deben derivarse de evidencia real del caso.

Lee primero `00_contexto_comun.md` (caso, evidencias, estándar visual, reglas de GitHub).

## Tu entregable de análisis 1: Contexto de uso

| Usuarios | Tareas | Entorno | Restricciones |
|---|---|---|---|
| ¿Quiénes y con qué capacidades? (usa E1, E2) | ¿Qué desean lograr? (reservar/reprogramar rápido) | ¿Dónde, cuándo, con qué dispositivo? (celular, en movimiento, E1/E8) | ¿Qué limita la interacción? (conexión variable E8, capacidades distintas E2) |

## Tu entregable de análisis 2: Persona y escenario

**Persona** (nombre ficticio + objetivo + comportamiento + capacidad/condición relevante + frustración + necesidad). Basa esto directamente en E1 y E2 — no inventes rasgos que no aporten a la tarea. Ejemplo de estructura (complétalo, no lo copies literal):
- Nombre: [ficticio]
- Objetivo: reservar una tutoría sin perder tiempo entre clases.
- Comportamiento: revisa el celular en momentos cortos (bus, pasillo).
- Capacidad/condición relevante: [ej. usa lector de pantalla, o simplemente conexión inestable].
- Frustración: procesos largos por WhatsApp (E4), confirmaciones que se pierden entre mensajes (E5).
- Necesidad: confirmación clara e inmediata.

**Escenario:** situación + contexto + desencadenante + objetivo + dificultad actual. No describas todavía pantallas, solo la situación real de hoy (proceso manual).

## Tu entregable de análisis 3: Journey map del proceso ACTUAL (5 etapas)

Completa esta tabla para las 5 etapas: Buscar, Contactar, Acordar, Confirmar, Cambiar.
En cada columna define: Acción, Pensamiento, Emoción, Problema, Oportunidad.

- Usa E4 (14 min, 9 mensajes) para "Buscar/Contactar".
- Usa E3 (confirmaciones ambiguas) para "Acordar/Confirmar".
- Usa E5 (confirmación mezclada con otros mensajes) para "Confirmar".
- Usa E7 (secretaria transcribe manualmente) donde aplique a "Cambiar".

## Tu entregable de análisis 4: 5 Requisitos de usuario

Estructura obligatoria para cada uno: **"La persona debe poder [acción], bajo [condición], para [resultado]."** Asocia cada requisito con una evidencia (E1–E10) y con la pantalla del prototipo donde se representa.

Ejemplo de forma (no de contenido final):
1. La persona debe poder ver los horarios disponibles de un docente, bajo baja conectividad, para decidir sin esperar una respuesta por mensaje. → E8 → Pantalla 2.
2. La persona debe poder confirmar una reserva, bajo una sola pantalla resumen, para no depender de mensajes sueltos. → E5 → Pantalla 3.
(Completa 3 más, cubriendo E1, E3, E10 como mínimo).

**Dónde lo guardas:** `docs/03_dcu_contexto.pdf` (contexto de uso + persona + escenario + journey map + requisitos, todo en un solo PDF exportado de FigJam).

## Tu pantalla: "3. Resumen y confirmación"

**Contenido mínimo obligatorio:**
- Docente, fecha, hora, modalidad (presencial/virtual) visibles antes de confirmar.
- Acción "Confirmar" (botón primario del estándar visual).
- Opción "Volver" (para corregir antes de confirmar).

**Conceptos que debes evidenciar:**
- **Reconocimiento** (no recordar): todos los datos de la reserva visibles en una sola pantalla, el usuario no debe recordar nada de pantallas anteriores.
- **Carga cognitiva:** no mostrar más información de la necesaria para decidir.
- **Retroalimentación:** un estado de "procesando" si la conexión tarda (referencia E8).
- **Corrección:** el botón "Volver" debe permitir corregir antes de confirmar (referencia directa a E10 — deshacer antes de confirmar definitivamente).

**Evidencia a citar:** E5 (confirmaciones que se pierden/mezclan), E10 (necesidad de corregir antes de confirmar), E8 (tolerancia a demoras de red).

## Checklist antes de dar por terminada tu parte

- [ ] Contexto de uso completo (las 4 columnas, sin genérico).
- [ ] Persona y escenario basados en E1/E2, sin biografía decorativa.
- [ ] Journey map con las 5 etapas y las 5 filas completas.
- [ ] 5 requisitos con la estructura exacta, cada uno con evidencia y pantalla asociada.
- [ ] Pantalla 3 muestra todos los datos de la reserva + confirmar + volver.
- [ ] Exportaste `docs/03_dcu_contexto.pdf`.
- [ ] Exportaste la captura de tu pantalla a `prototipo/capturas/`.

## Pasos exactos en GitHub

1. Crea el issue: **"DCU: contexto, persona, journey map, requisitos + pantalla Confirmación"**.
2. Crea la rama: `feature/dcu-contexto`.
3. Commit 1 (ejemplo): `Agrega contexto de uso, persona y escenario basados en E1 y E2`.
4. Commit 2 (ejemplo): `Agrega journey map, requisitos y pantalla Resumen y confirmacion`.
5. Abre el PR, título: "DCU + Pantalla Confirmación", vincula el issue (`Closes #N`).
6. Pide revisión a otro integrante.
