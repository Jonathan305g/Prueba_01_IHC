# Actividad 3: Comparación de Mecanismos de Agendamiento

## Matriz Comparativa

| Criterio | Agenda Digital Interna | Solicitud con Confirmación | Autoagendamiento | Mecanismo Híbrido |
| :--- | :--- | :--- | :--- | :--- |
| **Tiempo administrativo** | Alto (el personal digita todo manualmente). | Medio (requiere revisión y respuesta manual). | Mínimo (procesamiento automático). | Bajo (automatiza casos de rutina y filtra excepciones). |
| **Tiempo total de confirmación** | Inmediato si el paciente está presente; lento por WhatsApp. | Variable (depende de cuándo el personal revisa el mensaje). | Inmediato (confirmación instantánea en pantalla). | Inmediato para citas directas; breve para casos especiales. |
| **Acciones del paciente** | Mínimas (comunicar datos por mensaje o voz). | Medias (llenar formulario de solicitud y esperar). | Altas (buscar horario, ingresar datos y confirmar). | Moderadas según preferencia (autoservicio o asistencia). |
| **Acciones del personal** | Altas (buscar disponibilidad, anotar y notificar). | Medias (revisar solicitud, verificar agenda y responder). | Mínimas (solo atención médica, no administrativa). | Medias (atiende únicamente conflictos, dudas o excepciones). |
| **Intervención humana** | 100% manual. | Parcial (revisión obligatoria del 100% de solicitudes). | 0% manual. | Parcial/Baja (solo en reasignaciones o casos complejos). |
| **Prevención de conflictos** | Vulnerable al error humano o traslapes por doble agenda. | Reduce traslapes, pero propensa a demoras de respuesta. | Cero traslapes (bloqueo en tiempo real por base de datos). | Cero traslapes con flexibilidad ante imprevistos. |
| **Facilidad y accesibilidad** | Compleja para el personal; nula interacción digital del paciente. | Fácil para el paciente; requiere espera de respuesta. | Alta para usuarios digitales; barrera para adultos mayores. | Máxima adaptabilidad a todo perfil de paciente. |
| **Compatibilidad (5 fisioterapeutas)** | Difícil de coordinar entre 5 profesionales en paralelo. | Manejo centralizado pero propenso a cuellos de botella. | Excelente (sincroniza agendas individuales automáticamente). | Excelente (mantiene control de los 5 profesionales). |

## Selección y Justificación del Mecanismo

**Mecanismo Seleccionado:** **Mecanismo Híbrido**

El centro **GABO'S Readaptación y Movimiento** cuenta con 5 fisioterapeutas y atiende pacientes con distintos perfiles y niveles de competencia digital. Un autoagendamiento puro excluiría a pacientes no familiarizados con plataformas web, mientras que una agenda interna mantendría la sobrecarga administrativa y el cuello de botella en WhatsApp.

El mecanismo híbrido permite automatizar la mayoría de las citas de rutina mediante un portal web (autoagendamiento en tiempo real). Al mismo tiempo, conserva un canal asistido con un panel de control interno para que el personal gestione casos especiales, reprogramaciones complejas o pacientes que prefieren el contacto telefónico/WhatsApp. Esta integración garantiza cero traslapes en las agendas de los 5 profesionales, optimiza el tiempo operativo y asegura la accesibilidad total.

---

# Actividad 4: Operacionalización de la Eficiencia

| Operación | Inicio | Final | Criterio de Éxito | Acciones Observables | Errores Posibles |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Consultar disponibilidad** | El usuario selecciona la especialidad, servicio o fisioterapeuta deseado. | El sistema despliega en pantalla la rejilla de días y horarios libres sin conflictos. | Muestra la disponibilidad real en tiempo real en menos de 2 segundos. | Selección de profesional/servicio, actualización interactiva del calendario. | Calendario desactualizado, consulta colgada, no disponibilidad sin mensaje de advertencia. |
| **Registrar una cita** | El usuario selecciona un slot de horario disponible y presiona "Agendar". | Generación del comprobante/código de confirmación y envío de notificación. | Almacenamiento correcto en la base de datos y bloqueo instantáneo del horario. | Ingreso de datos personales, validación de formulario, clic en "Confirmar". | Sobrerreserva (*double booking*), campos obligatorios vacíos, error de conexión al guardar. |
| **Modificar una cita** | El usuario o personal ingresa al detalle de una cita agendada y elige "Modificar datos". | El sistema actualiza y guarda los nuevos datos de la cita con confirmación visual. | Actualización correcta de la ficha sin alterar la fecha u hora agendada. | Edición de campos (ej. motivo de consulta, contacto), clic en "Guardar cambios". | Pérdida de datos originales por fallo de guardado, inconsistencia en la ficha. |
| **Cancelar una cita** | El usuario o personal selecciona la opción "Cancelar cita". | El sistema libera el slot de horario en la agenda y emite la notificación de cancelación. | Cambio de estado a "Cancelada" y liberación inmediata del horario para otros usuarios. | Clic en cancelar, confirmación en modal de advertencia, motivo de cancelación. | Cancelación accidental por falta de confirmación, falla al liberar el slot liberado. |
| **Reagendar una cita** | El usuario o personal selecciona "Reagendar" sobre una cita activa. | Confirmación del nuevo horario bloqueado y actualización de la cita previa. | Liberación inmediata del horario anterior y asignación correcta del nuevo slot. | Selección de la nueva fecha/hora, confirmación del cambio. | Mantener bloqueado el horario antiguo, asignar un slot previamente ocupado. |