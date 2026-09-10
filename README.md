# 📋 PRUEBA PRÁCTICA: Diseño HCI de un Mecanismo para la Gestión de Citas
**Caso de Estudio:** GABO'S Readaptación y Movimiento  

---

## 🏛️ Información Institucional y Académica
* **Institución:** Universidad Técnica de Ambato (UTA)
* **Facultad:** Facultad de Ingeniería en Sistemas, Electrónica e Industrial (FISEI)
* **Carrera:** Software — 5to "A"
* **Ciclo Académico:** Agosto – Diciembre 2026
* **Asignatura:** Interacción Humano/Computador
* **Docente:** Ing. José Caiza, Mg.
* **Duración:** 120 minutos | **Valoración:** 3.0 Puntos

---

## 👥 Integrantes, Roles y Trazabilidad en GitHub

> **Nota de entrega:** Cada integrante debe registrar al menos **un Issue cerrado** y **dos commits significativos** (evitar cambios triviales de formato o mensajes genéricos como «actualización»).

| Integrante | Usuario GitHub | Rol HCI | Artefacto Asignado | Issue Cerrado | Commits Significativos |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Abril Lara Emilio Alexander** | `@EmilioAbril` | Analista de Procesos y Factores Humanos | Flujo AS-IS y Matriz de usuarios y necesidades (Act. 1 y 2) | [#1](https://github.com/Jonathan305g/Prueba_01_IHC/issues/1) | `feat(diagnostico)` |
| **Cusme Vélez Manuel Steven** | `@ManuelCusme` | Arquitecto de Mecanismos y Eficiencia | Comparación de mecanismos e Indicadores de eficiencia (Act. 3 y 4) | [#2](https://github.com/Jonathan305g/Prueba_01_IHC/issues/2) | `feat(mecanismos)` |
| **Gamboa Guamán Jonathan Alexis** | `@Jonathan305g` | Diseñador Conceptual HCI | Metáforas de interfaz y mapeo computacional (Act. 5) | [#3](https://github.com/Jonathan305g/Prueba_01_IHC/issues/3) | `feat(metaforas)` | 
| **Lozada Marcial Pablo Damián** | `@Idk-Damian` | Diseñador UI/UX y Prototipado | Prototipo interactivo navegable en Figma/Penpot (Act. 6) | [#4](https://github.com/Jonathan305g/Prueba_01_IHC/issues/4) | `feat(prototipo)` |
| **Martínez Jiménez William Fernando** | `@WilliamMartinez` | Evaluador de Usabilidad y Calidad | Protocolo de validación, informe final y síntesis (Act. 7 y 8) | [#5](https://github.com/Jonathan305g/Prueba_01_IHC/issues/5) | `docs(informe)` |
---

## 🎯 Desglose de Responsabilidades por Integrante

### 1. Abril Lara Emilio Alexander — Diagnóstico de Situación y Usuarios
* **Artefactos:** Flujo AS-IS, Matriz de usuarios y necesidades.
* **Entregables:**
  * Modelado del flujo actual AS-IS señalando tiempos muertos, transcripciones redundantes e inconsistencias entre Google Drive, WhatsApp y agenda física.
  * Análisis formal de al menos dos factores humanos (ej. sobrecarga cognitiva del recepcionista, fallas de memoria de trabajo) y dos factores tecnológicos (ej. asincronía de canales, ausencia de concurrencia/persistencia).
  * Matriz completa de usuarios: Paciente, 5 Fisioterapeutas, Personal administrativo y Administrador del centro.

### 2. Cusme Vélez Manuel Steven — Mecanismos y Eficiencia Operacional 
* **Artefactos:** Comparación de mecanismos, Indicadores de eficiencia.
* **Entregables:**
  * Matriz comparativa multicriterio (Agenda digital interna, Solicitud con confirmación, Autoagendamiento y Mecanismo híbrido) considerando tiempos, accesibilidad, prevención de solapamientos para los 5 especialistas y privacidad.
  * Selección argumentada del mecanismo idóneo para el centro.
  * Operacionalización de la variable dependiente (*Eficiencia del proceso*) con delimitación de inicio, fin, acciones observables, errores y criterios de éxito para: consulta, registro, modificación, cancelación y reagendamiento.

### 3. Gamboa Guamán Jonathan Alexis — Metáforas de Interfaz y Modelo Mental 
* **Artefactos:** Metáforas de interfaz (organizacional, navegación y funcional).
* **Entregables:**
  * Diseño de 3 metáforas de interfaz: una organizacional/familiar (ej. casillero/pizarra por terapeuta), una de navegación (ej. ruta/línea de tiempo) y una funcional (ej. ticket canjeable).
  * Matriz de mapeo: Dominio fuente ➡️ Elemento digital ➡️ Etiqueta ➡️ Comportamiento ➡️ Riesgo cultural/límite.
  * Definición de affordances, visibilidad del estado del sistema, feedback, reglas de negocio y persistencia computacional.

### 4. Lozada Marcial Pablo Damián — Prototipado Interactivo 
* **Artefactos:** Prototipo de fidelidad media navegable.
* **Entregables:**
  * Flujos completos en Figma/Penpot: Inicio, consulta de disponibilidad, filtro entre los 5 terapeutas, captura de datos, confirmación/resumen, detalle de cita, reagendamiento y diálogo destructivo de cancelación.
  * Cumplimiento estricto de heurísticas: Navegación reversible sin pérdida de datos, estados visibles (carga, éxito, error por conflicto de horario), contraste de color adecuado y soporte de navegación por teclado.
  * Enlace público interactivo con permisos abiertos de visualización.

### 5. Martínez Jiménez William Fernando — Protocolo de Validación e Integración 
* **Artefactos:** Protocolo de validación, Recomendación final e Informe técnico consolidado.
* **Entregables:**
  * Protocolo de evaluación con 3 participantes (P1, P2, P3) midiendo éxito, tiempo, acciones, intervenciones y errores en las 5 tareas clave.
  * Justificación técnica final diferenciando decisiones fundamentadas de preferencias subjetivas.
  * Control de calidad y ensamblaje del documento PDF final (máximo 5 páginas).

---

## 🔗 Entregables y Enlaces del Proyecto

* **Actividades 1 y 2 (Diagnóstico y Usuarios):** [Documento Actividad 1 y 2](docs/01_analisis_actual/actividad_1_2.md)
* **Actividades 3 y 4 (Mecanismos y Eficiencia):** [Documento Actividad 3 y 4](02-mecanismos-eficiencia/mecanismos_eficiencia.md)
* **Actividad 5 (Metáforas de Interfaz):** [Documento Actividad 5](03-metaforas-interfaz/metaforas-interfaz.md)
* **Actividad 6 (Prototipo Interactivo Figma):** [Ver Prototipo Interactivo en Figma](https://www.figma.com/proto/gabo-salud-ihc/GABOS-Gestion-Citas-Prototipo) | [Especificación Prototipo](04-prototipo-figma/prototipo-interactivo.md) | [Enlaces y Capturas](docs/04_prototipo/figma_links.md)
* **Informe Técnico Consolidado (PDF):** [Ver Informe Final](informe-final/)

---

## ⏱️ Cronograma de Ejecución Recomendado 

| Intervalo | Fase | Acciones de Trabajo |
| :--- | :--- | :--- |
| **00 – 15 min** | Alineación de Equipo | Acordar mecanismo base, crear el repositorio, crear los Issues (#1 al #5) y asignar ramas de trabajo. |
| **15 – 70 min** | Construcción Paralela | - Abril: Flujo AS-IS y usuarios.<br>- Cusme: Matrices de decisión e indicadores.<br>- Gamboa: Mapeo de metáforas.<br>- Lozada: Diseño y cableado de pantallas en Figma.<br>- Martínez: Estructuración del protocolo e informe (PDF). |
| **70 – 95 min** | Revisión y Control de HCI | Lozada comparte el prototipo; Gamboa y Cusme verifican consistencia de metáforas e indicadores en el prototipo; primeros commits documentados. |
| **95 – 110 min** | Pruebas y Redacción Final | Martínez simula la validación con el prototipo, redacta la recomendación final y cierra su Issue; commits finales de cada integrante. |
| **110 – 120 min** | Cierre y Verificación | Cierre de Issues restantes, verificación de permisos públicos en Figma y exportación del PDF (máximo 5 páginas). |
