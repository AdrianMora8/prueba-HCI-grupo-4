# Integrante 3 — Diseño Centrado en el Usuario (DCU)
**Estudiante / Asignado:** CristianDDGA  
**Issue:** [#3](https://github.com/AdrianMora8/prueba-HCI-grupo-4/issues/3)  
**Proyecto:** Tutoría Fácil UTA  

---

## 1. Contexto de uso

| Usuarios | Tareas | Entorno | Restricciones |
|---|---|---|---|
| Estudiantes universitarios de la UTA con diversas capacidades motrices/visuales (ej. uso con una mano en movimiento, o lectores de pantalla y navegación por teclado E2) y distintos hábitos tecnológicos (E1, E2). | Consultar disponibilidad de docentes, reservar tutorías académicas y solicitar reprogramaciones de citas de forma autónoma y rápida. | Dispositivos móviles (smartphones) utilizados en movimiento o espacios de tránsito (transporte público/bus, pasillos de la facultad entre clases) (E1, E8). | Conexión a internet inestable o de velocidad variable durante desplazamientos (E8), tiempos cortos entre actividades académicas y diversas capacidades de interacción (E2). |

---

## 2. Persona y escenario

### Persona
* **Nombre:** Laura Mendoza (basada en patrones de E1 y E2)
* **Objetivo:** Reservar una tutoría académica en menos de 2 minutos sin perder tiempo entre clases ni depender de respuestas manuales.
* **Comportamiento:** Revisa y opera su teléfono móvil en lapsos breves mientras viaja en el bus urbano o camina por los pasillos de la facultad.
* **Capacidad / Condición relevante:** Uso del dispositivo con una sola mano en movimiento y conexión de datos móviles variable (E1, E8).
* **Frustración:** Procesos largos de coordinación por WhatsApp (E4), respuestas demoradas y confirmaciones que se pierden entre múltiples chats (E5).
* **Necesidad:** Confirmación clara, inmediata y centralizada de su cita sin ambigüedades.

### Escenario (Proceso Manual Actual)
Laura se encuentra en el bus rumbo a la facultad a las 11:45 AM. Recuerda que necesita una tutoría con su docente de programación para resolver dudas antes del examen de la próxima semana. Abre WhatsApp y le escribe un mensaje al profesor consultando sus horarios disponibles. Durante el trayecto, el bus pierde señal momentáneamente y el docente tarda varios minutos en responder. Cuando por fin responde, le propone dos horarios, pero uno choca con la clase de Laura. Ella vuelve a responder sugiriendo otro horario y queda a la espera de que el docente revise su agenda personal y le confirme. Tras 14 minutos y 9 mensajes cruzados, el docente le responde "Listo, dale". Laura no sabe con certeza si la cita quedó agendada formalmente o en qué aula será, y la confirmación queda traspapelada entre decenas de chats de compañeros.

---

## 3. Journey map del proceso ACTUAL (5 etapas)

| Dimensión | 1. Buscar | 2. Contactar | 3. Acordar | 4. Confirmar | 5. Cambiar |
|---|---|---|---|---|---|
| **Acción** | Revisa su horario de clases en el celular y busca el contacto del docente en WhatsApp. | Envía un mensaje inicial al docente solicitando espacio para tutoría académica. | Intercambia mensajes proponiendo y descartando horarios según disponibilidad. | Recibe respuesta del docente ("Listo", "Ok") y asume agendada la cita. | Escribe de nuevo al docente o secretaria para pedir cambio de hora por un imprevisto. |
| **Pensamiento** | *"Ojalá el docente tenga un espacio libre hoy o mañana a primera hora."* | *"Espero que lea rápido el mensaje antes de que llegue a la facultad."* | *"Ese horario se cruza con mi clase, debo proponerle otra hora."* | *"¿Habrá quedado anotado en su agenda oficial o se le olvidará?"* | *"Qué vergüenza molestar otra vez por WhatsApp para cambiar la hora."* |
| **Emoción** | 😐 Ansiedad / Incertidumbre | ⏳ Impaciencia | 😤 Frustración / Agotamiento | ❓ Confusión / Desconfianza | 🤦‍♀️ Estrés / Incomodidad |
| **Problema** | No existe una agenda centralizada pública con horarios disponibles. | Proceso lento y asíncrono; tiempo promedio de 14 min y 9 mensajes (E4). | Respuestas ambiguas y riesgo de seleccionar horarios ya ocupados (E3). | La confirmación se pierde o mezcla entre múltiples chats de WhatsApp (E5). | Requerir transcripción manual por la secretaria o renegociar desde cero (E7). |
| **Oportunidad** | Mostrar disponibilidad docente en tiempo real accesible desde el móvil. | Permitir reserva directa en un clic sin intercambio de mensajes directos. | Bloquear automáticamente horarios ocupados y diferenciar estados. | Generar una pantalla de resumen e indicación inequívoca de confirmación. | Ofrecer una opción directa de "Reprogramar" que libere el cupo anterior automáticamente. |

---

## 4. 5 Requisitos de usuario

1. **La persona debe poder** consultar la lista de horarios disponibles de un docente en tiempo real, **bajo** condiciones de red lenta o conexión móvil variable, **para** seleccionar un cupo sin esperar respuestas por mensaje de texto.  
   * **Evidencia:** E8, E1  
   * **Pantalla asociada:** Pantalla 2 (Docente y horario)

2. **La persona debe poder** revisar la totalidad de los datos de la cita (docente, fecha, hora y modalidad) en una única pantalla de resumen previa, **bajo** una vista clara que evite depender de la memoria, **para** verificar la información antes de procesar la reserva.  
   * **Evidencia:** E5, E9  
   * **Pantalla asociada:** Pantalla 3 (Resumen y confirmación)

3. **La persona debe poder** deshacer o corregir la selección de horario y modalidad mediante un botón "Volver" visible, **bajo** el flujo de confirmación antes del registro definitivo, **para** evitar errores de reserva accidental sin perder la navegación.  
   * **Evidencia:** E10, E3  
   * **Pantalla asociada:** Pantalla 3 (Resumen y confirmación)

4. **La persona debe poder** obtener un comprobante con estado inequívoco ("Confirmado") y detalles completos de su tutoría, **bajo** una interfaz libre de ambigüedades, **para** no depender de mensajes sueltos que puedan traspapelarse.  
   * **Evidencia:** E3, E5  
   * **Pantalla asociada:** Pantalla 4 (Confirmada y reprogramación)

5. **La persona debe poder** navegar la interfaz utilizando teclado o tecnologías de asistencia (lector de pantalla), **bajo** etiquetas claras y alto contraste visual, **para** completar su reserva independientemente de sus capacidades motrices o de visión.  
   * **Evidencia:** E2  
   * **Pantalla asociada:** Pantalla 1 (Inicio) y Pantalla 2 (Horario)
