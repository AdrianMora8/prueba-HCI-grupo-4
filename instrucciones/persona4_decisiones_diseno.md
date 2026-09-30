# Integrante 4 — Decisiones de diseño + Guía de estilo + Pantalla "Confirmada y reprogramación"

> **Instrucciones para IA:** si vas a usar un asistente de IA, pégale este archivo
> completo junto con `00_contexto_comun.md`. Pídele ayuda para justificar (con
> lenguaje de diseño, no genérico) por qué cada decisión resuelve una evidencia
> específica de E1–E10. No debe proponer iconografía o metáforas nuevas fuera de
> las ya sugeridas (calendario, agenda, tarjeta de cita).

Lee primero `00_contexto_comun.md` (caso, evidencias, estándar visual, reglas de GitHub).

**Tu issue:** [#4](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/4) — asignado a MatiusJBG.

## ⚠️ Tarea prioritaria (hazla primero, en los primeros 10-15 minutos)

A ti te toca crear el **archivo único de Figma del equipo** (ver sección "Cómo
trabajamos todos en el mismo Figma" en `00_contexto_comun.md`):

1. Crea el archivo en Figma.
2. Comparte acceso de edición con los otros 3 integrantes (Share → Invite por
   correo/usuario, o link con "Anyone with the link can edit").
3. Dentro de ese mismo archivo, crea una página **"🎨 Componentes"** con los
   componentes reales (no dibujos sueltos) del estándar visual: botón
   primario/secundario, campo de texto (normal/foco/error), tarjeta de horario
   (disponible/ocupado/seleccionado), tarjeta de tutoría, mensaje de estado. Los
   demás deben usar **instancias** de estos componentes en sus pantallas, nunca
   redibujarlos.
4. Avisa al grupo en cuanto el archivo y los componentes estén listos, y pega el
   enlace en `prototipo/enlace_prototipo.md`.

## Tu entregable de análisis 1: Decisiones de diseño

Completa la tabla exacta, citando la evidencia indicada (no cambies las evidencias, ya están definidas por el caso):

| Concepto | Decisión solicitada | Evidencia |
|---|---|---|
| Metáfora | Selecciona calendario, agenda, tarjeta de cita u otra metáfora y explica el modelo mental que aprovecha | E9 |
| Affordance y mapeo | Explica por qué un horario parece seleccionable y cómo la acción se relaciona con el resultado | E3 y E9 |
| Manipulación directa | Permite seleccionar o cambiar un horario actuando sobre el objeto visible | E10 |
| Retroalimentación | Muestra estados de carga, selección, confirmación y error con texto comprensible | E3, E5 y E8 |
| Carga cognitiva | Prioriza información, limita opciones simultáneas, evita que la persona memorice datos | E4 y E5 |
| Gestalt | Aplica y justifica al menos 3 leyes entre proximidad, semejanza, continuidad, cierre, figura-fondo y destino común | Diseño (justificación propia, visible en las 4 pantallas) |
| Riesgo cultural | No dependas de un ícono, color o símbolo cuyo significado pueda ser ambiguo | E2 y E9 |

## Tu entregable de análisis 2: Guía de estilo (formaliza el estándar ya definido)

Documenta esto en el PDF (ya está decidido, tu trabajo es formalizarlo y verificar que las 4 pantallas lo cumplan):

- **Tipografía:** jerarquía título/subtítulo/cuerpo/auxiliar (valores en `00_contexto_comun.md`).
- **Color:** acción principal, fondo, texto, éxito, error — recuerda que los estados siempre llevan texto o ícono con etiqueta, nunca solo color (E2, E9).
- **Componentes:** botón, campo, horario disponible, tarjeta de tutoría, mensaje de estado.
- **Consistencia:** mismas etiquetas, misma ubicación de acciones, misma respuesta del sistema en las 4 pantallas — **revisa las pantallas 1, 2 y 3 de tus compañeros y anota cualquier inconsistencia antes de cerrar tu PR.**

**Dónde lo guardas:** `docs/04_decisiones_diseno.pdf` (tabla de decisiones + guía de estilo).

## Tu pantalla: "4. Confirmada y reprogramación"

**Contenido mínimo obligatorio:**
- Estado inequívoco de "Confirmado" (texto + ícono, componente de mensaje de estado).
- Datos de la cita visibles (docente, fecha, hora).
- Entrada clara para iniciar el cambio de horario (reprogramar).

**Conceptos que debes evidenciar:**
- **Visibilidad del estado:** que quede claro e inconfundible que la reserva ya está confirmada (contra E5, confirmaciones que se pierden).
- **Recuperación:** la reprogramación debe ser fácil de encontrar y ejecutar, no escondida.
- **Manipulación directa:** reprogramar se hace actuando sobre el horario visible, igual que en la pantalla 2, no con un formulario aparte.

**Evidencia a citar:** E5 (confirmaciones perdidas → aquí se resuelve con estado inequívoco), E10 (posibilidad de corregir/cambiar), E7 (evitar que la info quede desactualizada — la reprogramación debe reflejarse de inmediato).

## Tarea compartida que coordinas tú: prueba cruzada + iteración

1. Entrega el prototipo YA CONECTADO (las 4 pantallas) a una persona de otro equipo, sin explicarle cómo funciona.
2. Pídele: "reserva una tutoría para el jueves y luego cambia el horario".
3. Registra: si completó la tarea, tiempo aproximado, error u duda observable, comentario final.
4. Aplica una mejora concreta relacionada con el hallazgo (guarda captura antes/después).
5. Documenta todo en `evaluacion/prueba_iteracion.md` (tarea, participante, resultado, tiempo, hallazgo, antes, después).
6. Haz el commit de esa mejora vinculado al issue/PR correspondiente.

## Checklist antes de dar por terminada tu parte

- [ ] Página "🎨 Componentes" creada y compartida ANTES de que los demás empiecen sus pantallas.
- [ ] Tabla de decisiones de diseño completa con las evidencias exactas indicadas.
- [ ] Guía de estilo documentada y verificada contra las 4 pantallas reales (no solo la tuya).
- [ ] Pantalla 4 muestra estado confirmado + datos + entrada a reprogramar.
- [ ] Prueba cruzada ejecutada y documentada en `evaluacion/prueba_iteracion.md`.
- [ ] Exportaste `docs/04_decisiones_diseno.pdf`.
- [ ] Exportaste la captura de tu pantalla a `prototipo/capturas/`.

## Pasos exactos en GitHub

1. El issue ya existe: [#4](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/4) "Decisiones de diseño + guía de estilo + pantalla Confirmada/Reprogramación".
2. Crea tu propia rama: `feature/decisiones-diseno` (desde `main`, créala tú).
3. Commit 1 (ejemplo): `Agrega tabla de decisiones de diseno y guia de estilo`.
4. Commit 2 (ejemplo): `Agrega pantalla Confirmada y reprogramacion con estado inequivoco`.
5. (Commit opcional 3, si haces la iteración): `Agrega hallazgo y mejora de la prueba cruzada`.
6. Abre el PR, título: "Decisiones de diseño + Pantalla Confirmación", vincula el issue (`Closes #4`).
7. Pide revisión a otro integrante.
