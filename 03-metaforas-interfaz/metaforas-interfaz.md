# Metáforas de Interfaz y Mapeo Computacional — GABO'S Readaptación y Movimiento

**Responsable:** Gamboa Guamán Jonathan Alexis ([@Jonathan305g](https://github.com/Jonathan305g))
**Actividad:** 5 | **Ruta:** `docs/03_metaforas_hci/`

---

## 1. Introducción

Las metáforas de interfaz permiten que el usuario entienda un sistema nuevo relacionándolo con algo que ya conoce del mundo físico. En GABO'S, el modelo mental actual de pacientes y personal está basado en **objetos y rutinas físicas**: una agenda de papel, casilleros, turnos y comprobantes en mano. Por eso se proponen 3 metáforas que traducen ese mundo físico a la interfaz digital, sin romper la forma en que las personas ya piensan el proceso.

---

## 2. Las 3 metáforas

### 2.1 Metáfora organizacional — Casillero por terapeuta

**Idea central:** cada uno de los 5 fisioterapeutas tiene su propio "casillero" visual (como una casilla de correo o un locker), donde se acumulan sus citas del día/semana.

**Problema de usabilidad que resuelve:** en el flujo AS-IS, no existe una vista consolidada de las 5 agendas; la información vive dispersa entre agenda física y Drive. El casillero le da a cada terapeuta —y a quien agenda— un **contenedor único e identificable por persona**, evitando que las citas de distintos profesionales se mezclen visualmente.

**Cómo se ve en pantalla:** una fila o grilla de 5 tarjetas grandes (una por terapeuta, con foto/nombre), y dentro de cada una las citas del día apiladas como fichas dentro del casillero.

---

### 2.2 Metáfora de navegación — Ruta tipo mapa/pasos

**Idea central:** agendar una cita se representa como **avanzar por un camino con paradas marcadas** (como un mapa de ruta o un GPS con hitos), donde cada "parada" es un paso del proceso: elegir terapeuta → elegir horario → llenar datos → confirmar.

**Problema de usabilidad que resuelve:** en el flujo actual el paciente no sabe "en qué parte" del proceso está ni cuánto falta (todo ocurre por mensajes sueltos de WhatsApp sin estructura). La ruta le da **visibilidad constante del progreso** y permite retroceder a una parada anterior sin perder lo ya recorrido.

**Cómo se ve en pantalla:** una barra superior tipo mapa con 4 puntos/hitos conectados por una línea; el punto actual resaltado, los completados marcados como "visitados", y los pendientes en gris.

---

### 2.3 Metáfora funcional — Comprobante/recibo

**Idea central:** al confirmar una cita, el sistema entrega un **comprobante digital**, igual que un recibo físico que uno guarda como prueba de una transacción.

**Problema de usabilidad que resuelve:** hoy la "confirmación" es un mensaje de texto informal en WhatsApp que se pierde entre otros chats y no sirve como respaldo. El comprobante da un **objeto de cierre claro y verificable**, con toda la información de la cita en un solo lugar consultable después.

**Cómo se ve en pantalla:** una tarjeta tipo recibo con folio/código de cita, nombre del paciente, terapeuta asignado, fecha, hora y un botón para "guardar" o "compartir" el comprobante.

---

## 3. Matriz de mapeo computacional

| Dominio fuente (mundo físico) | Elemento digital | Etiqueta en la interfaz | Comportamiento | Riesgo cultural / límite |
|---|---|---|---|---|
| Casillero físico de correspondencia | Tarjeta/panel por terapeuta | "Agenda de [Nombre del terapeuta]" | Al tocar el casillero, se expande mostrando las citas asignadas a ese terapeuta ese día | Si un paciente ve el casillero de otro paciente dentro del mismo terapeuta, no debe exponerse el nombre completo de terceros (riesgo de privacidad) |
| Mapa de ruta con paradas (GPS) | Barra de progreso con hitos | "Paso 1 de 4: Elegir terapeuta" | El hito actual se resalta; los anteriores quedan marcados como completados y son clicables para regresar | El usuario podría asumir que retroceder "borra" el progreso siguiente, cuando en realidad los datos deben conservarse (debe comunicarse claramente que no se pierde información) |
| Recibo/comprobante de compra | Tarjeta de confirmación con folio | "Comprobante de cita #[folio]" | Se genera automáticamente al finalizar el paso de confirmación; queda accesible en el detalle de la cita | Un comprobante sugiere una transacción "cerrada e inmutable"; debe dejarse claro que la cita aún puede reagendarse o cancelarse después, para no confundir al paciente pensando que ya no puede modificarla |
| Pizarra de turnos (referencia complementaria) | Indicador de estado por horario | "Disponible" / "Reservado" / "Bloqueado" | Cambia de color según el estado en tiempo real | Debe evitarse el uso exclusivo de color (ej. rojo/verde) sin texto o ícono, para no excluir a usuarios con daltonismo |

---

## 4. Affordances, visibilidad, consistencia y retroalimentación

**Affordances:**
- El casillero se ve "tocable/expandible" mediante una sombra o borde que sugiere que es un contenedor con más contenido dentro.
- Los hitos de la ruta que ya se completaron se muestran con un ícono de check, sugiriendo que se puede volver a ellos.
- El comprobante incluye un ícono de descarga/compartir reconocible, sugiriendo que es un objeto que se puede guardar.

**Visibilidad del estado del sistema:**
- La ruta siempre muestra en qué paso está el usuario y cuántos faltan — nunca deja al usuario "perdido" sin saber cuánto avanzó.
- Cada casillero muestra un contador visible de citas del día, sin necesidad de abrirlo.
- Los horarios muestran su estado (disponible/reservado/bloqueado) de forma permanente, no solo al hacer clic.

**Consistencia:**
- El color y forma usados para "disponible", "reservado" y "bloqueado" se mantienen iguales en todas las pantallas (selector de horario, resumen, detalle de cita).
- La metáfora de ruta se usa únicamente para procesos de varios pasos (agendar, reagendar); no se reutiliza para acciones de un solo paso (como cancelar), evitando sobrecargar el modelo mental del usuario con una metáfora que no aplica.

**Retroalimentación inmediata:**
- Al seleccionar un horario dentro de un casillero, este se resalta instantáneamente antes de avanzar al siguiente paso.
- Al confirmar una cita, el comprobante aparece de inmediato (no hay espera ni ambigüedad de "¿ya se guardó o no?").
- Si un horario deja de estar disponible mientras el paciente lo estaba seleccionando (conflicto de concurrencia), el sistema debe notificarlo en el momento, antes de permitir avanzar al siguiente paso de la ruta.

---

## 5. Reglas de validación, estados y persistencia

### Estados de un horario (dentro del casillero de cada terapeuta)

| Estado | Significado | Regla de validación |
|---|---|---|
| **Disponible** | Nadie ha reservado ese horario con ese terapeuta | Puede ser seleccionado libremente por un paciente |
| **Reservado** | Ya existe una cita confirmada en ese horario | No puede seleccionarse; el sistema debe bloquear el clic y mostrar el motivo |
| **Bloqueado** | El terapeuta no atiende ese horario (día libre, hora de almuerzo, etc.) | No puede seleccionarse bajo ninguna circunstancia; se distingue visualmente del estado "reservado" para no confundir causas |

### Persistencia computacional que sostiene las metáforas

- **Persistencia de progreso en la ruta:** si el paciente cierra la pestaña a mitad del proceso de agendamiento, los datos ya ingresados (terapeuta elegido, horario seleccionado) deben mantenerse guardados temporalmente para no obligarlo a repetir todo desde el paso 1.
- **Persistencia del comprobante:** una vez generado, el comprobante debe quedar almacenado de forma permanente y accesible desde el "detalle de cita", incluso si la cita se reagenda posteriormente (debe conservarse el historial, no sobrescribirse silenciosamente).
- **Consistencia entre casilleros:** el estado de un horario (disponible/reservado/bloqueado) debe reflejarse igual para todos los usuarios que consulten el mismo casillero al mismo tiempo, evitando que dos pacientes distintos vean el mismo horario como "disponible" y ambos intenten reservarlo (esto resuelve directamente el problema de concurrencia identificado en el diagnóstico AS-IS).

---

## 6. Verificación en el Prototipo Interactivo (Actividad 6)

Las 3 metáforas conceptuales diseñadas en este artefacto se ven reflejadas directamente en los flujos y pantallas del prototipo interactivo navegable desarrollado en Figma:

1. **Metáfora del Casillero por Terapeuta (Organizacional):**
   - Implementada en el **Selector de los 5 Fisioterapeutas** ([`04-prototipo-figma/capturas/imagen4.jpeg`](../04-prototipo-figma/capturas/imagen4.jpeg)) y la **Grilla de disponibilidad** ([`imagen3.jpeg`](../04-prototipo-figma/capturas/imagen3.jpeg)), asignando un casillero/contenedor exclusivo a cada especialista.
2. **Metáfora de Ruta tipo Mapa/Pasos (Navegación):**
   - Implementada como la barra de progreso superior de 4 hitos en el **Formulario del Paciente** ([`04-prototipo-figma/capturas/imagen5.jpeg`](../04-prototipo-figma/capturas/imagen5.jpeg)) y en la pantalla de **Resumen** ([`imagen6.jpeg`](../04-prototipo-figma/capturas/imagen6.jpeg)), brindando visibilidad constante del trayecto y soporte para navegación reversible.
3. **Metáfora Funcional de Comprobante/Recibo (Funcional):**
   - Implementada en el **Resumen provisional `#GB-TMP-2026`** ([`imagen6.jpeg`](../04-prototipo-figma/capturas/imagen6.jpeg)) y en la vista del **Detalle de Cita Confirmada `#GB-8841`** ([`imagen7.jpeg`](../04-prototipo-figma/capturas/imagen7.jpeg)), otorgando un objeto de confirmación verificable con folio único.

> 🔗 **Documentación y prototipo interactivo:** [`docs/04_prototipo/figma_links.md`](../docs/04_prototipo/figma_links.md) | [`04-prototipo-figma/prototipo-interactivo.md`](../04-prototipo-figma/prototipo-interactivo.md)