# Validación de Usabilidad e Informe de Resultados

**Responsable:** Martínez Jiménez William Fernando  
**Actividad:** 7 — Protocolo de validación  
**Caso:** GABO'S Readaptación y Movimiento  

---

## 1. Objetivo de la validación

La validación tiene como objetivo evaluar el comportamiento del prototipo
de gestión de citas de GABO'S Readaptación y Movimiento durante la ejecución
de las principales tareas del proceso de agendamiento.

La evaluación considera no únicamente el tiempo requerido para completar
cada tarea, sino también el número de acciones realizadas, los errores
cometidos, la necesidad de intervención y el éxito alcanzado.

De esta manera se analiza la eficiencia del proceso desde una perspectiva
de Interacción Humano-Computador, verificando además la claridad de la
navegación, la visibilidad del estado del sistema, la prevención de errores
y la capacidad de recuperación del usuario.

---

## 2. Participantes

Para la validación se consideraron tres perfiles representativos con
diferentes niveles de familiaridad con sistemas digitales.

| Participante | Perfil | Familiaridad digital |
|---|---|---|
| **P1** | Usuario joven acostumbrado al uso de aplicaciones móviles, reservas y plataformas web. | Alta |
| **P2** | Usuario adulto con experiencia en sistemas administrativos y aplicaciones de uso cotidiano. | Media - Alta |
| **P3** | Usuario adulto mayor que utiliza principalmente WhatsApp, llamadas y funciones básicas del teléfono. | Básica |

La diferencia entre los perfiles permite observar si el prototipo mantiene
un nivel adecuado de comprensión para usuarios con distinta experiencia digital.

---

## 3. Tareas evaluadas

Cada participante realizó las siguientes tareas sobre el prototipo:

1. Encontrar un horario disponible.
2. Registrar una nueva cita.
3. Cambiar la fecha o el fisioterapeuta de una cita existente.
4. Cancelar una cita.
5. Agendar nuevamente una cita después de una cancelación.

Las tareas representan las operaciones principales contempladas dentro del
sistema de gestión de citas.

---

## 4. Indicadores registrados

Durante cada tarea se registraron los siguientes indicadores:

- **Éxito:** indica si el participante consiguió completar correctamente la tarea.
- **Tiempo:** duración total desde el inicio hasta la finalización.
- **Acciones:** número aproximado de clics, selecciones o entradas necesarias.
- **Intervención:** cantidad de ocasiones en las que fue necesario proporcionar ayuda.
- **Errores:** acciones incorrectas o decisiones que desviaron temporalmente al usuario.

Estos indicadores permiten analizar la eficiencia sin utilizar el tiempo
como único criterio.

---

## 5. Resultados de la validación

| Participante | Tarea | Éxito | Tiempo | Acciones | Intervención | Errores |
|---|---|---:|---:|---:|---:|---:|
| P1 | Encontrar horario disponible | Sí | 32 s | 5 | 0 | 0 |
| P1 | Registrar cita | Sí | 78 s | 12 | 0 | 0 |
| P1 | Cambiar fecha/especialista | Sí | 64 s | 8 | 0 | 0 |
| P1 | Cancelar cita | Sí | 24 s | 3 | 0 | 0 |
| P1 | Agendar nuevamente | Sí | 70 s | 9 | 0 | 0 |
| P2 | Encontrar horario disponible | Sí | 27 s | 4 | 0 | 0 |
| P2 | Registrar cita | Sí | 68 s | 11 | 0 | 0 |
| P2 | Cambiar fecha/especialista | Sí | 51 s | 7 | 0 | 0 |
| P2 | Cancelar cita | Sí | 21 s | 3 | 0 | 0 |
| P2 | Agendar nuevamente | Sí | 58 s | 8 | 0 | 0 |
| P3 | Encontrar horario disponible | Sí | 55 s | 7 | 0 | 0 |
| P3 | Registrar cita | Sí | 112 s | 15 | 1 | 1 |
| P3 | Cambiar fecha/especialista | Sí | 96 s | 11 | 1 | 1 |
| P3 | Cancelar cita | Sí | 33 s | 4 | 0 | 0 |
| P3 | Agendar nuevamente | Sí | 105 s | 12 | 1 | 1 |

---

## 6. Resultados generales

Las quince tareas definidas fueron completadas correctamente por los
participantes.

De las quince ejecuciones realizadas:

- **15 de 15 tareas fueron completadas:** tasa de éxito del 100 %.
- **12 de 15 tareas fueron realizadas sin ayuda:** autonomía del 80 %.
- **3 tareas necesitaron una intervención breve:** 20 % de las ejecuciones.
- Se identificaron **3 errores recuperables**, todos concentrados en el
  participante con menor familiaridad digital.
- Ningún error produjo pérdida de información, cancelaciones accidentales
  ni reservas duplicadas.

El tiempo promedio aproximado de ejecución fue de **59,6 segundos por tarea**.

Los resultados evidencian que la interacción resulta directa para usuarios
con experiencia digital alta o media. El participante P3 necesitó mayor
tiempo y apoyo principalmente durante el registro y el reagendamiento,
donde se requiere interpretar más información y completar varias decisiones.

---

## 7. Análisis de resultados

### 7.1 Consulta de disponibilidad

La consulta de disponibilidad fue comprendida correctamente por los tres
participantes. Los usuarios P1 y P2 identificaron rápidamente los horarios
libres gracias a la estructura de la grilla y a las etiquetas
**Disponible** y **Reservado**.

P3 necesitó más tiempo para revisar las columnas correspondientes a días y
horarios, aunque consiguió realizar la tarea sin ayuda.

Se considera conveniente mantener las etiquetas textuales de estado y no
depender únicamente de diferencias de color.

---

### 7.2 Registro de una nueva cita

El registro fue una de las tareas que requirió mayor tiempo debido a la
cantidad de información que debe ingresar el paciente.

P1 y P2 completaron el formulario sin intervención. P3 necesitó una breve
orientación durante el ingreso de información.

El uso de etiquetas permanentes como **Cédula**, **Nombres completos**,
**WhatsApp/Teléfono**, **Correo** y **Motivo de consulta** facilita el
reconocimiento de los datos requeridos.

Como mejora se recomienda incorporar validaciones inmediatas junto a cada
campo y mensajes breves que indiquen claramente cómo corregir un dato
incorrecto.

---

### 7.3 Modificación y reagendamiento

La opción **Reagendar Fecha / Especialista** fue comprendida por los
participantes.

Un elemento importante del flujo es el mensaje:

> El horario previo no se libera hasta confirmar.

Este comportamiento evita que el usuario pierda accidentalmente su turno
actual mientras busca una nueva opción.

El nuevo horario debe validarse antes de sustituir definitivamente al
anterior, evitando estados inconsistentes o dos citas activas simultáneamente.

---

### 7.4 Cancelación de la cita

La cancelación fue la tarea con menor tiempo de ejecución y no produjo
errores en ninguno de los participantes.

El diálogo de confirmación informa claramente la consecuencia de la acción
antes de ejecutarla y presenta dos alternativas diferenciadas:

- **No, mantener cita**
- **Sí, cancelar cita**

La confirmación explícita reduce el riesgo de cancelaciones accidentales y
mantiene el control del usuario sobre una operación destructiva.

---

### 7.5 Agendamiento posterior a una cancelación

Los tres participantes consiguieron iniciar nuevamente el proceso después
de cancelar una cita.

P3 requirió una breve intervención para identificar nuevamente el recorrido
de disponibilidad, especialista y confirmación.

Este resultado evidencia la importancia de mantener una estructura de
navegación consistente entre el registro inicial y posteriores operaciones
de reagendamiento.

---

## 8. Hallazgos y oportunidades de mejora

| Hallazgo | Evidencia observada | Recomendación |
|---|---|---|
| La disponibilidad es reconocible rápidamente. | P1 y P2 encontraron horario en menos de 35 segundos. | Mantener texto visible junto con el estado del horario. |
| El formulario concentra mayor carga de interacción. | P3 necesitó ayuda y cometió un error recuperable. | Añadir validación en línea y ejemplos breves. |
| La ruta de pasos facilita la orientación. | Los usuarios reconocieron el paso de Datos del Paciente y Confirmación. | Mostrar la misma barra desde Disponibilidad y Especialista. |
| El reagendamiento protege el turno original. | El banner informa que el horario previo no se libera inmediatamente. | Mantener esta regla antes de confirmar el nuevo horario. |
| La cancelación presenta buena prevención de errores. | 3 de 3 participantes cancelaron sin equivocarse. | Mantener el diálogo de confirmación y la acción segura para volver. |

---

# Actividad 8: Recomendación Final

## 9. Mecanismo recomendado

Se recomienda implementar un **mecanismo híbrido de gestión de citas** para
GABO'S Readaptación y Movimiento.

El mecanismo permite automatizar las operaciones habituales mediante el
portal de agendamiento y mantener intervención del personal administrativo
en casos que necesitan asistencia.

Los pacientes capaces de utilizar la plataforma pueden:

- consultar disponibilidad;
- seleccionar un fisioterapeuta;
- registrar sus datos;
- confirmar una cita;
- consultar una reserva existente;
- reagendar;
- cancelar.

Paralelamente, el centro puede mantener atención asistida mediante
WhatsApp, teléfono o personal de recepción para usuarios que no puedan o
no deseen utilizar directamente el portal.

---

## 10. Justificación de la decisión

La selección del mecanismo híbrido no corresponde únicamente a una
preferencia por una interfaz digital.

La decisión se sustenta en las características del proceso y en los
resultados de la evaluación.

### Frente a una agenda digital interna

Una agenda gestionada únicamente por el personal continúa concentrando las
tareas administrativas en recepción. El mecanismo híbrido reduce esta carga
permitiendo que parte de los pacientes gestione directamente sus citas.

### Frente a la solicitud con confirmación

El modelo de solicitud mantiene una espera entre el envío de la petición y
la revisión del personal. El portal permite confirmar inmediatamente los
casos que cumplen las reglas de disponibilidad.

### Frente al autoagendamiento completamente automático

Un sistema exclusivamente automático puede representar una barrera para
pacientes con poca experiencia digital.

Los resultados obtenidos con P3 evidencian que algunos usuarios pueden
necesitar orientación adicional.

Por esta razón, conservar un canal asistido resulta coherente con la
diversidad de usuarios del centro.

---

## 11. Relación con los principios de HCI

La solución propuesta mantiene los siguientes principios:

- **Visibilidad del estado del sistema:** los horarios y citas presentan
  estados explícitos como Disponible, Reservado y Confirmada.
- **Prevención de errores:** los horarios ocupados se bloquean y las
  cancelaciones requieren confirmación.
- **Control y libertad:** el usuario puede regresar y modificar decisiones
  antes de confirmar.
- **Consistencia:** las acciones y estados mantienen las mismas etiquetas
  durante el proceso.
- **Reconocimiento antes que recuerdo:** disponibilidad, especialista,
  datos y estado permanecen visibles.
- **Retroalimentación:** el sistema informa la confirmación, los conflictos
  y las consecuencias de las acciones.
- **Accesibilidad:** la información textual acompaña a los colores y las
  acciones utilizan etiquetas comprensibles.

---

## 12. Conclusión

La validación permitió comprobar que el prototipo cubre adecuadamente las
principales operaciones de gestión de citas planteadas para GABO'S
Readaptación y Movimiento.

Los participantes pudieron consultar horarios, registrar citas, modificar
reservas, cancelar y volver a agendar.

Las mayores dificultades se concentraron en el participante con menor
familiaridad digital, especialmente en operaciones que contienen más pasos
o campos de información.

Por ello, el mecanismo híbrido resulta adecuado para el contexto: mejora la
eficiencia de las operaciones normales sin eliminar la asistencia humana
necesaria para excepciones o usuarios con mayores dificultades digitales.

La propuesta permite reducir transcripciones manuales, aumentar la
visibilidad de la disponibilidad, prevenir conflictos de agenda y mantener
un proceso de interacción más claro, consistente y trazable.
