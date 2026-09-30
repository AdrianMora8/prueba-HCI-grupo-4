# Integrante 1 — Fundamentos de IHC + Pantalla "Inicio y búsqueda"

> **Instrucciones para IA:** si vas a usar un asistente de IA para ayudarte, pégale
> este archivo completo junto con `00_contexto_comun.md` y pídele que redacte
> contigo cada sección respetando SOLO las evidencias E1–E10 listadas ahí. No debe
> inventar datos, usuarios ni funciones fuera del alcance descrito.

Lee primero `00_contexto_comun.md` (caso, evidencias, estándar visual, reglas de GitHub).

## Tu entregable de análisis: Matriz humano-sistema

Completa esta tabla exacta. Sé concreto, una frase por celda, citando evidencia cuando aplique.

| Elemento | Pregunta orientadora | Qué debes responder |
|---|---|---|
| Personas | ¿Quién interactúa directa o indirectamente y qué objetivo tiene? | Identifica al estudiante (primario) y docente/secretaría (secundarios). Usa E1 y E6/E7. |
| Sistema | ¿Qué procesa, almacena o comunica la solución? | Disponibilidad, reserva, estado, cambio de horario. |
| Entrada y salida | ¿Qué acciones entrega la persona y qué respuesta devuelve el sistema? | Selección, confirmación, mensajes, estados, errores. Usa E3 y E8 (conexión variable → el sistema debe responder algo comprensible aunque tarde). |
| Disciplinas de apoyo | ¿Cómo aportan informática, psicología cognitiva, ergonomía y diseño? | Un aporte concreto y distinto por cada una de las 4 disciplinas (no genérico). |
| Interacción | ¿Qué estilos se usarán y por qué? | Menús, formularios y manipulación directa de horarios. Justifica por qué (referencia E1: uso desde el celular en movimiento). |

**Dónde lo guardas:** `docs/01_matriz_ihc.pdf` (exporta la tabla desde FigJam a PDF).

## Tu pantalla: "1. Inicio y búsqueda"

**Contenido mínimo obligatorio:**
- Objetivo claro de la pantalla (qué puede hacer el usuario aquí, en una frase visible).
- Acceso a "Reservar" (acción principal, botón primario del estándar visual).
- Acceso a "Mis tutorías" (acción secundaria).

**Conceptos que el diseño debe evidenciar (y que debes poder explicar si te preguntan):**
- **Jerarquía visual:** el botón de reservar debe destacar más que cualquier otro elemento (tamaño/color/posición).
- **Figura-fondo:** los elementos accionables deben distinguirse claramente del fondo.
- **Consistencia:** usa exactamente los componentes y colores del estándar visual común, no crees botones nuevos.
- **Navegación:** debe quedar claro cómo se llega a la pantalla 2 (Docente y horario).

**Evidencia a citar en tu justificación de diseño:** E1 (uso móvil en contexto de movimiento, necesita ser rápido) y E4 (el proceso actual tarda 14 min / 9 mensajes — tu pantalla debe reducir pasos desde el inicio).

## Checklist antes de dar por terminada tu parte

- [ ] Matriz completa, sin celdas vacías, con al menos 2 referencias a E1–E10.
- [ ] Pantalla 1 usa componentes del sistema de diseño común (no colores/botones propios).
- [ ] El flujo de la pantalla 1 conecta visualmente hacia la pantalla 2.
- [ ] Exportaste la matriz como `docs/01_matriz_ihc.pdf`.
- [ ] Exportaste la captura de tu pantalla a `prototipo/capturas/`.

## Pasos exactos en GitHub

1. Crea el issue: **"Fundamentos de IHC: matriz humano-sistema + pantalla Inicio"**, descripción: "Completar matriz humano-sistema (docs/01_matriz_ihc.pdf) y construir pantalla 1 Inicio y búsqueda en el prototipo, según guía de estilo común."
2. Crea la rama: `feature/fundamentos-ihc`.
3. Commit 1 (ejemplo): `Agrega matriz humano-sistema con evidencias E1, E4 y E6`.
4. Commit 2 (ejemplo): `Agrega pantalla Inicio y busqueda con componentes del sistema de diseno`.
5. Abre el PR desde `feature/fundamentos-ihc` hacia `main`, título: "Fundamentos de IHC + Pantalla Inicio", descripción con el issue vinculado (`Closes #N`).
6. Pide revisión a otro integrante (no seas tú quien apruebe tu propio PR).
