# Integrante 3 — Diseño Centrado en el Usuario (DCU) (análisis, sin Figma)

> **Instrucciones para IA:** si vas a usar un asistente de IA, pégale este archivo
> completo junto con `00_contexto_comun.md`. Pídele ayuda para redactar la persona,
> el escenario y el journey map, pero recuérdale explícitamente: "no inventes una
> biografía extensa, la persona debe representar patrones de E1-E10, no rasgos
> decorativos". Tu resultado final debe ser lo bastante específico para que OTRA
> persona, sin hablar contigo, pueda construir la pantalla correcta en Figma solo
> leyendo tu documento.

Lee primero `00_contexto_comun.md` (caso, evidencias, estándar visual, reglas de GitHub, y cómo está dividido el trabajo).

**Tu issue:** [#3](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/3) — asignado a CristianDDGA.

**Importante:** tú NO construyes ninguna pantalla. Tu trabajo es análisis + dejar
especificaciones tan claras que la persona 4 (quien construye el prototipo completo)
pueda implementarlas sin preguntarte nada.

## Parte A — Contexto de uso

| Usuarios | Tareas | Entorno | Restricciones |
|---|---|---|---|
| ¿Quiénes y con qué capacidades? (usa E1, E2) | ¿Qué desean lograr? (reservar/reprogramar rápido) | ¿Dónde, cuándo, con qué dispositivo? (celular, en movimiento, E1/E8) | ¿Qué limita la interacción? (conexión variable E8, capacidades distintas E2) |

## Parte B — Persona y escenario

**Persona** (nombre ficticio + objetivo + comportamiento + capacidad/condición relevante + frustración + necesidad). Basa esto directamente en E1 y E2 — no inventes rasgos que no aporten a la tarea. Ejemplo de estructura (complétalo, no lo copies literal):
- Nombre: [ficticio]
- Objetivo: reservar una tutoría sin perder tiempo entre clases.
- Comportamiento: revisa el celular en momentos cortos (bus, pasillo).
- Capacidad/condición relevante: [ej. usa lector de pantalla, o simplemente conexión inestable].
- Frustración: procesos largos por WhatsApp (E4), confirmaciones que se pierden entre mensajes (E5).
- Necesidad: confirmación clara e inmediata.

**Escenario:** situación + contexto + desencadenante + objetivo + dificultad actual. No describas todavía pantallas, solo la situación real de hoy (proceso manual).

## Parte C — Journey map del proceso ACTUAL (5 etapas)

Completa esta tabla para las 5 etapas: Buscar, Contactar, Acordar, Confirmar, Cambiar.
En cada columna define: Acción, Pensamiento, Emoción, Problema, Oportunidad.

- Usa E4 (14 min, 9 mensajes) para "Buscar/Contactar".
- Usa E3 (confirmaciones ambiguas) para "Acordar/Confirmar".
- Usa E5 (confirmación mezclada con otros mensajes) para "Confirmar".
- Usa E7 (secretaria transcribe manualmente) donde aplique a "Cambiar".

## Parte D — 5 Requisitos de usuario

Estructura obligatoria para cada uno: **"La persona debe poder [acción], bajo [condición], para [resultado]."** Asocia cada requisito con una evidencia (E1–E10) y con la pantalla del prototipo donde se representa (usa la tabla de las 4 pantallas en `00_contexto_comun.md`).

Ejemplo de forma (no de contenido final):
1. La persona debe poder ver los horarios disponibles de un docente, bajo baja conectividad, para decidir sin esperar una respuesta por mensaje. → E8 → Pantalla 2.
2. La persona debe poder confirmar una reserva, bajo una sola pantalla resumen, para no depender de mensajes sueltos. → E5 → Pantalla 3.
(Completa 3 más, cubriendo E1, E3, E10 como mínimo).

## Especificaciones para el prototipo (esto es lo que persona 4 va a implementar)

Para cada uno de tus 5 requisitos, escribe una instrucción de una frase dirigida a
quien construye, indicando exactamente qué debe contener la pantalla que
corresponde. Ejemplo de formato: *"Requisito 2 → Pantalla 3: mostrar docente, fecha,
hora y modalidad juntos en una tarjeta resumen antes del botón Confirmar, sin que
el usuario tenga que volver a la pantalla anterior — por E5."*

**Dónde lo guardas:** `docs/03_dcu_contexto.pdf` (contexto de uso + persona + escenario + journey map + requisitos + especificaciones para el prototipo, todo en un solo PDF).

## Checklist antes de dar por terminada tu parte

- [ ] Contexto de uso completo (las 4 columnas, sin genérico).
- [ ] Persona y escenario basados en E1/E2, sin biografía decorativa.
- [ ] Journey map con las 5 etapas y las 5 filas completas.
- [ ] 5 requisitos con la estructura exacta, cada uno con evidencia y pantalla asociada.
- [ ] Especificaciones por pantalla redactadas para que persona 4 no tenga que interpretar nada.
- [ ] Exportaste `docs/03_dcu_contexto.pdf`.

## Pasos exactos en GitHub

1. El issue ya existe: [#3](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/3) "DCU: contexto, persona, journey map, requisitos".
2. Crea tu propia rama: `feature/dcu-contexto` (desde `main`, créala tú).
3. Commit 1 (ejemplo): `Agrega contexto de uso, persona y escenario basados en E1 y E2`.
4. Commit 2 (ejemplo): `Agrega journey map, requisitos y especificaciones para el prototipo`.
5. Abre el PR, título: "DCU", vincula el issue (`Closes #3`).
6. Pide revisión a otro integrante.
