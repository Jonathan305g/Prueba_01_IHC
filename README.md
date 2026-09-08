# 📋 PRUEBA PRÁCTICA HCI: Sistema de Gestión de Citas
**Caso:** GABO'S Readaptación y Movimiento  
**Asignatura:** Interacción Humano-Computador — 5to Semestre  
**Duración base:** 120 min | **Valor:** 3.0 Puntos  
**Entregables finales:**
1. **Informe técnico (PDF):** Máximo 5 páginas (análisis, matrices, operacionalización, metáforas y justificación).
2. **Prototipo interactivo navegable:** Enlace público en Figma o Penpot.

---

## 👥 Reparto de Trabajo y Responsabilidades (5 Integrantes)

| Integrante | Rol Principal | Actividades Asignadas | Ponderación Rúbrica |
| :--- | :--- | :--- | :--- |
| **Integrante 1** | Analista de Procesos y Factores Humanos | **Actividad 1 & Actividad 2** | 0.65 pts |
| **Integrante 2** | Arquitecto de Mecanismos y Eficiencia | **Actividad 3 & Actividad 4** | 0.75 pts |
| **Integrante 3** | Diseñador Conceptual HCI | **Actividad 5** | 0.65 pts |
| **Integrante 4** | Prototipador UI/UX (Figma/Penpot) | **Actividad 6** | 0.70 pts |
| **Integrante 5** | Evaluador de Usabilidad y Cierre Técnico | **Actividad 7 & Actividad 8** | 0.25 pts (+ Integración) |

---

### 👤 INTEGRANTE 1: Diagnóstico de Situación y Usuarios
* **Actividades:** 1 (Analizar proceso actual) y 2 (Identificar usuarios y necesidades).
* **Entregables específicos:**
  1. **Diagrama/Flujo AS-IS detallado:** Identificar actores, datos de entrada/salida y puntos críticos (cuellos de botella por WhatsApp, transcripción manual, desincronización con Drive).
  2. **Análisis de fricciones:**
     - Tiempos muertos y esperas.
     - Fallos de retroalimentación y visibilidad de estado del sistema.
  3. **Factores Clave:**
     - *2 Factores Humanos:* Carga cognitiva del recepcionista, fatiga por cambio de contexto mental (agenda de papel vs. chat), estrés por doble reserva.
     - *2 Factores Tecnológicos:* Canales asíncronos no integrados, falta de persistencia y concurrencia de datos.
  4. **Matriz de Usuarios y Necesidades completada:**
     - Paciente, Fisioterapeuta (5 profesionales), Personal administrativo y Administrador del centro.

---

### 👤 INTEGRANTE 2: Comparación Técnica y Métricas de Eficiencia
* **Actividades:** 3 (Comparar mecanismos de agendamiento) y 4 (Operacionalizar la eficiencia).
* **Entregables específicos:**
  1. **Matriz de Decisión Multicriterio:**
     - Comparar las 4 opciones: *Agenda digital interna*, *Solicitud con confirmación*, *Autoagendamiento* y *Mecanismo híbrido*.
     - Parámetros: Tiempo administrativo, acciones por usuario, prevención de solapamientos para los 5 fisioterapeutas, accesibilidad y factibilidad.
  2. **Selección del Mecanismo:** Justificar técnicamente la opción recomendada (ej. Enfoque híbrido o autoagendamiento con reglas de negocio).
  3. **Matriz de Operacionalización de la Eficiencia:**
     - Delimitar Inicio, Final, Criterio de éxito, Acciones observables y Errores potenciales para:
       * *Consultar disponibilidad*
       * *Registrar cita*
       * *Modificar cita*
       * *Cancelar cita*
       * *Reagendar cita*
     - Definir la fórmula o métrica cuantitativa/cualitativa de la variable dependiente (Eficiencia del proceso).

---

### 👤 INTEGRANTE 3: Modelo Mental y Metáforas de Interfaz
* **Actividades:** 5 (Construir metáforas de interfaz).
* **Entregables específicos:**
  1. **Selección y diseño de al menos 3 metáforas:**
     - Metáfora organizacional/familiar (ej. *El Casillero/Pizarra de turnos por especialista*, *La Ficha clínica de mesa*).
     - Metáfora de navegación (ej. *Ruta de rehabilitación paso a paso*, *Línea de tiempo continua*).
     - Tercera metáfora complementaria funcional (ej. *Boleto/Ticket de confirmación canjeable*).
  2. **Matriz de Mapeo Semántico y Técnico:**
     - Dominio fuente ➡️ Elemento digital ➡️ Etiqueta/Mensaje ➡️ Comportamiento ➡️ Riesgo cultural/límite.
  3. **Fundamentación Teórica HCI:**
     - Resolver problemas de usabilidad identificados en el AS-IS.
     - Definir affordances, visibilidad, consistencia, estados del sistema (vacío, ocupado, en proceso) y retroalimentación inmediata.
     - Diseñar las reglas de persistencia para evitar que las metáforas rompan el modelo mental del usuario.

---

### 👤 INTEGRANTE 4: Construcción del Prototipo Navegable
* **Actividades:** 6 (Elaborar el prototipo interactivo en Figma o Penpot).
* **Entregables específicos:**
  1. **Wireframes / Prototipo funcional navegable:**
     - Pantalla 1: Inicio de gestión y selector de fisioterapeutas (filtro por los 5 especialistas).
     - Pantalla 2: Vista de cuadrícula/calendario de disponibilidad en tiempo real.
     - Pantalla 3: Formulario accesible de ingreso de datos del paciente.
     - Pantalla 4: Resumen pre-confirmación y modal de éxito/ticket.
     - Pantalla 5: Vista de detalle de cita existente.
     - Pantalla 6: Flujo de Reagendamiento (cambio de fecha/hora manteniendo consistencia).
     - Pantalla 7: Cancelación con confirmación destructiva en 2 pasos y diálogo de recuperación.
  2. **Requisitos de interacción HCI obligatorios:**
     - Navegación bidireccional (volver atrás sin borrar datos del formulario).
     - Estados de feedback: *Loading (carga)*, *Success (éxito)*, *Error (solapamiento)* y *Empty states*.
     - Accesibilidad visual: Alto contraste, etiquetas visibles y navegación lógica.
  3. Generar el **enlace público con permisos de visualización**.

---

### 👤 INTEGRANTE 5: Protocolo de Validación, Recomendación y Ensamblaje
* **Actividades:** 7 (Validación con usuarios), 8 (Recomendación final) + **Control de Calidad del Documento**.
* **Entregables específicos:**
  1. **Protocolo de Pruebas de Usabilidad:**
     - Estructurar la prueba para 3 participantes representativos (P1: Paciente adulto, P2: Paciente joven, P3: Recepcionista).
     - Medición sobre las 5 tareas requeridas (búsqueda, registro, modificación, cancelación y reagendamiento posterior).
     - Matriz con: Tasa de éxito, tiempo por tarea, conteo de clics/acciones, nivel de intervención requerido y errores cometidos.
  2. **Recomendación y Justificación Final:**
     - Redacción de la conclusión técnica diferenciando preferencias subjetivas de evidencia empírica/HCI (viabilidad para 5 fisioterapeutas, baja carga para recepción).
  3. **Edición General:** Ensamblar las secciones de los 5 integrantes en el PDF final (estricto cumplimiento del límite de 5 páginas).

---

## ⏱️ Cronograma de Ejecución Sugerido (Bloque de 120 min)

| Minutos | Fase | Tareas Principales |
| :--- | :--- | :--- |
| **00 – 15** | Alineación Inicial | Lectura conjunta, acuerdos de diseño y definición de la alternativa a prototipar. |
| **15 – 65** | Trabajo en Paralelo | - Int 1: Redacta AS-IS y matriz de usuarios.<br>- Int 2: Matriz de mecanismos e indicadores.<br>- Int 3: Fichas de metáforas.<br>- Int 4: Estructuración y diseño del prototipo en Figma.<br>- Int 5: Matriz de validación y estructura del documento. |
| **65 – 90** | Punto de Control | Int 4 comparte el enlace interactivo; Int 3 valida que las metáforas estén reflejadas; Int 2 revisa el flujo de eficiencia. |
| **90 – 110** | Validación y Cierre | Int 5 realiza prueba rápida con el prototipo navegable y documenta la recomendación. |
| **110 – 120**| Exportación y Entrega | Consolidación del PDF (máx. 5 páginas), verificación de permisos del link de Figma y entrega. |

---

## 📌 Checklist de Entrega
- [ ] Enlace a Figma/Penpot probado en modo incógnito (acceso público para visualización).
- [ ] PDF con máximo 5 páginas.
- [ ] Rúbrica cubierta: Factores humanos/tecnológicos, matriz multicriterio, operacionalización, metáforas justificadas, prototipo navegable y plan de validación.
