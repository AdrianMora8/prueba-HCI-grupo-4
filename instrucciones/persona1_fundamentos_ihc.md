# Integrante 1 — Fundamentos de IHC + Pantalla "Inicio y búsqueda"

> **Instrucciones para IA:** si vas a usar un asistente de IA para ayudarte, pégale
> este archivo completo junto con `00_contexto_comun.md` y pídele que redacte
> contigo cada sección respetando SOLO las evidencias E1–E10 listadas ahí. No debe
> inventar datos, usuarios ni funciones fuera del alcance descrito.

Lee primero `00_contexto_comun.md` (caso, evidencias, estándar visual, reglas de GitHub).

**Tu issue:** [#1](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/1) — asignado a AdrianMora8.

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

## Prompt para la IA de Figma (pega esto directo, solo construye TU pantalla)

```
Diseña UNA sola pantalla móvil (375x812px) para la app "Tutoría Fácil UTA", una
app para reservar tutorías académicas. Esta pantalla es "Inicio y búsqueda", la
primera de un flujo de 4 pantallas — no diseñes las otras 3.

Sistema de diseño a usar (si ya existen estos componentes en el archivo, reutilízalos;
si no, créalos con estos valores exactos):
- Tipografía: familia sans-serif tipo Inter. Título 20px bold, Subtítulo 16px
  semibold, Cuerpo 14px regular, Auxiliar 12px regular gris #6B6B6B.
- Color: acción principal #2F6FED, fondo #FFFFFF, texto #1A1A1A.
- Grid de espaciado de 8px, márgenes laterales 16px.

Contenido obligatorio de esta pantalla:
- Encabezado con el nombre de la app y un mensaje corto del objetivo ("Reserva tu
  tutoría en minutos").
- Botón primario grande "Reservar tutoría" (el elemento más prominente de toda
  la pantalla — máxima jerarquía visual).
- Acceso secundario "Mis tutorías" (botón o tarjeta menos prominente).
- Sin campos de login ni formularios. Layout limpio, mucho espacio en blanco.

Principios a aplicar: jerarquía visual clara (el botón principal debe destacar
sobre todo lo demás), figura-fondo (los elementos accionables deben distinguirse
claramente del fondo), consistencia (usa exactamente los colores y tipografía de
arriba, no inventes otros).

Nombra el frame "01-Inicio". En Prototype mode, deja preparada la interacción:
tap en "Reservar tutoría" → navega al frame "02-Horario" (ese frame lo construye
otro integrante del equipo en el mismo archivo; si aún no existe, deja la
interacción pendiente de conectar).

Fidelidad baja-media: sin ilustraciones ni fotos reales, solo bloques, tarjetas y
tipografía bien jerarquizada.
```

## Checklist antes de dar por terminada tu parte

- [ ] Matriz completa, sin celdas vacías, con al menos 2 referencias a E1–E10.
- [ ] Pantalla 1 usa componentes del sistema de diseño común (no colores/botones propios).
- [ ] El flujo de la pantalla 1 conecta visualmente hacia la pantalla 2.
- [ ] Exportaste la matriz como `docs/01_matriz_ihc.pdf`.
- [ ] Exportaste la captura de tu pantalla a `prototipo/capturas/`.

## Pasos exactos en GitHub

1. El issue ya existe: [#1](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/1) "Fundamentos de IHC: matriz humano-sistema + pantalla Inicio".
2. Crea tu propia rama: `feature/fundamentos-ihc` (desde `main`, créala tú).
3. Commit 1 (ejemplo): `Agrega matriz humano-sistema con evidencias E1, E4 y E6`.
4. Commit 2 (ejemplo): `Agrega pantalla Inicio y busqueda con componentes del sistema de diseno`.
5. Abre el PR desde `feature/fundamentos-ihc` hacia `main`, título: "Fundamentos de IHC + Pantalla Inicio", descripción con el issue vinculado (`Closes #1`).
6. Pide revisión a otro integrante (no seas tú quien apruebe tu propio PR).
