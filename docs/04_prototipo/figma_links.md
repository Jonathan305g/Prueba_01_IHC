# Prototipo Interactivo Navegable — Figma / Penpot

**Responsable:** Lozada Marcial Pablo Damián ([@Idk-Damian](https://github.com/Idk-Damian))  
**Artefacto:** Actividad 6 — Prototipado Interactivo  
**Ruta:** `docs/04_prototipo/figma_links.md`  

---

## 🔗 Enlace Público al Prototipo Interactivos

> **Acceso directo en Figma (Permisos Abiertos de Visualización):**  
> 🔗 [Ver Prototipo Interactivo Navegable en Figma](https://www.figma.com/proto/gabo-salud-ihc/GABOS-Gestion-Citas-Prototipo)

---

## 📱 Mapeo de Flujos y Pantallas Obligatorias

El prototipo abarca los 8 flujos requeridos por la prueba práctica, garantizando navegabilidad reversible, accesibilidad visual y visibilidad del estado del sistema:

| # | Pantalla / Flujo Obligatorio | Descripción en el Prototipo | Captura de Pantalla |
|---|---|---|---|
| **1** | **Inicio de gestión** | Pantalla principal de acceso donde el paciente elige entre agendar nueva cita o consultar/modificar cita existente. | ![Inicio de Gestión](capturas/imagen1.jpeg) |
| **2** | **Consulta de disponibilidad** | Grilla interactiva semanal con filtros por fecha, especialista y tipo de terapia, diferenciando estados disponible y reservado. | ![Consulta de Disponibilidad](capturas/imagen3.jpeg) |
| **3** | **Selector de los 5 fisioterapeutas** | Catálogo visual con las tarjetas de los 5 profesionales del centro y su disponibilidad inmediata. | ![Selector de Fisioterapeutas](capturas/imagen4.jpeg) |
| **4** | **Formulario de datos del paciente** | Formulario accesible para ingreso de Cédula, Nombres, WhatsApp, Correo y Motivo, con navegación hacia atrás sin pérdida de datos. | ![Formulario del Paciente](capturas/imagen5.jpeg) |
| **5** | **Resumen y confirmación de cita** | Comprobante temporal con bloqueo de horario por 10 minutos (#GB-TMP-2026) y botón de confirmación definitiva. | ![Resumen y Confirmación](capturas/imagen6.jpeg) |
| **6** | **Detalle de cita existente** | Vista del comprobante definitivo (#GB-8841) accesible mediante búsqueda por cédula o código, con opciones para reagendar o cancelar. | ![Detalle de Cita](capturas/imagen7.jpeg) |
| **7** | **Reagendamiento** | Flujo de selección de nuevo horario sin liberar el cupo anterior hasta confirmar el cambio. | ![Reagendamiento](capturas/imagen8.jpeg) |
| **8** | **Confirmación destructiva de cancelación** | Modal de alta visibilidad con advertencia explicita y confirmación en dos pasos para liberar el turno. | ![Cancelación Destructiva](capturas/imagen9.jpeg) |

---

## 🛠️ Instrucciones de Navegación e Interacción

1. Abrir el enlace navegable de Figma.
2. Hacer clic en **"Comenzar Reserva"** para iniciar el flujo principal de agendamiento.
3. Utilizar el botón **"← Atrás"** en cualquier paso del formulario para comprobar la navegación reversible sin pérdida de campos digitados.
4. Para la gestión de citas existentes, ingresar con el código `#GB-8841` para probar el reagendamiento o la cancelación con confirmación destructiva.
