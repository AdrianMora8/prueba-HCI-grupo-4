# Integrante 1 — Fundamentos de IHC + Decisiones de diseño (análisis, sin Figma)

> **Instrucciones para IA:** si vas a usar un asistente de IA, pégale este archivo
> completo junto con `00_contexto_comun.md`. Pídele que redacte contigo cada
> sección respetando SOLO las evidencias E1–E10 listadas ahí. No debe inventar
> datos, usuarios ni funciones fuera del alcance descrito. Tu resultado final debe
> ser lo bastante específico para que OTRA persona, sin hablar contigo, pueda
> construir la pantalla correcta en Figma solo leyendo tu documento.

Lee primero `00_contexto_comun.md` (caso, evidencias, estándar visual, reglas de GitHub, y cómo está dividido el trabajo).

**Tu issue:** [#1](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/1) — asignado a AdrianMora8.

**Importante:** tú NO construyes ninguna pantalla. Tu trabajo es análisis + dejar
especificaciones tan claras que la persona 4 (quien construye el prototipo completo)
pueda implementarlas sin preguntarte nada.

## Parte A — Matriz humano-sistema

Completa esta tabla exacta. Sé concreto, una frase por celda, citando evidencia cuando aplique.

| Elemento | Pregunta orientadora | Qué debes responder |
|---|---|---|
| Personas | ¿Quién interactúa directa o indirectamente y qué objetivo tiene? | Identifica al estudiante (primario) y docente/secretaría (secundarios). Usa E1 y E6/E7. |
| Sistema | ¿Qué procesa, almacena o comunica la solución? | Disponibilidad, reserva, estado, cambio de horario. |
| Entrada y salida | ¿Qué acciones entrega la persona y qué respuesta devuelve el sistema? | Selección, confirmación, mensajes, estados, errores. Usa E3 y E8 (conexión variable → el sistema debe responder algo comprensible aunque tarde). |
| Disciplinas de apoyo | ¿Cómo aportan informática, psicología cognitiva, ergonomía y diseño? | Un aporte concreto y distinto por cada una de las 4 disciplinas (no genérico). |
| Interacción | ¿Qué estilos se usarán y por qué? | Menús, formularios y manipulación directa de horarios. Justifica por qué (referencia E1: uso desde el celular en movimiento). |

## Parte B — Decisiones de diseño

Completa la tabla exacta, citando la evidencia indicada (no cambies las evidencias, ya están definidas por el caso):

| Concepto | Decisión solicitada | Evidencia |
|---|---|---|
| Metáfora | Selecciona calendario, agenda, tarjeta de cita u otra metáfora y explica el modelo mental que aprovecha | E9 |
| Affordance y mapeo | Explica por qué un horario parece seleccionable y cómo la acción se relaciona con el resultado | E3 y E9 |
| Manipulación directa | Permite seleccionar o cambiar un horario actuando sobre el objeto visible | E10 |
| Retroalimentación | Muestra estados de carga, selección, confirmación y error con texto comprensible | E3, E5 y E8 |
| Carga cognitiva | Prioriza información, limita opciones simultáneas, evita que la persona memorice datos | E4 y E5 |
| Gestalt | Aplica y justifica al menos 3 leyes entre proximidad, semejanza, continuidad, cierre, figura-fondo y destino común | Diseño (justificación propia) |
| Riesgo cultural | No dependas de un ícono, color o símbolo cuyo significado pueda ser ambiguo | E2 y E9 |

## Especificaciones para el prototipo (esto es lo que persona 4 va a implementar)

Escribe, para cada fila de las dos tablas de arriba, una instrucción de una frase
dirigida a quien construye, indicando en QUÉ PANTALLA aplica (usa la tabla de las 4
pantallas en `00_contexto_comun.md`):

- Ejemplo de formato: *"Metáfora: usar tarjeta de cita en la Pantalla 3 (Resumen y
  confirmación), mostrando docente/fecha/hora como en una tarjeta física — aplica
  por E9."*
- Cubre obligatoriamente: en qué pantalla va el calendario/metáfora elegida, en qué
  pantalla se nota el affordance del horario seleccionable, dónde se ve la
  manipulación directa, dónde aparecen los mensajes de retroalimentación (carga,
  error, éxito), qué se elimina/oculta para bajar la carga cognitiva, cuáles 3 leyes
  Gestalt se aplican y en qué pantalla se ve cada una, y qué ícono o color evitar
  por riesgo cultural.

**Dónde lo guardas:** `docs/01_matriz_ihc.pdf` (matriz humano-sistema) y
`docs/04_decisiones_diseno.pdf` (decisiones de diseño + especificaciones para el
prototipo).

## Checklist antes de dar por terminada tu parte

- [ ] Matriz humano-sistema completa, con al menos 2 referencias a E1–E10.
- [ ] Tabla de decisiones de diseño completa con las evidencias exactas indicadas.
- [ ] Especificaciones por pantalla redactadas (no solo la tabla teórica) para que
      persona 4 no tenga que interpretar nada.
- [ ] Exportaste `docs/01_matriz_ihc.pdf` y `docs/04_decisiones_diseno.pdf`.

## Pasos exactos en GitHub

1. El issue ya existe: [#1](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/1) "Fundamentos de IHC + Decisiones de diseño".
2. Crea tu propia rama: `feature/fundamentos-y-decisiones-diseno` (desde `main`, créala tú).
3. Commit 1 (ejemplo): `Agrega matriz humano-sistema con evidencias E1, E4 y E6`.
4. Commit 2 (ejemplo): `Agrega decisiones de diseno y especificaciones por pantalla para el prototipo`.
5. Abre el PR, título: "Fundamentos de IHC + Decisiones de diseño", descripción con el issue vinculado (`Closes #1`).
6. Pide revisión a otro integrante (no seas tú quien apruebe tu propio PR).
