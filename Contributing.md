# Guía de Contribución — GABO'S Gestión de Citas

Esta guía define cómo trabajamos en el repositorio: cómo crear Issues, cómo escribir commits significativos y cómo hacer Pull Requests. Es obligatorio seguirla para cumplir con la rúbrica de evidencia en GitHub.

---

## 📌 1. Issues

Cada integrante debe crear y cerrar **al menos un Issue** correspondiente a su artefacto asignado.

### Plantilla para crear un Issue

```markdown
### 🎯 Objetivo
[Descripción corta de lo que se va a entregar]

### 👤 Responsable
@usuario-github

### Artefacto
[Ej: Flujo AS-IS y Matriz de usuarios y necesidades]

### Criterios de aceptación
- [ ] Punto 1 a cumplir
- [ ] Punto 2 a cumplir
- [ ] Punto 3 a cumplir

### Referencias
[Documento de la prueba práctica / carpeta relacionada]
```

### Issues base del proyecto (crear al inicio)

| # | Título | Responsable |
|---|--------|-------------|
| #1 | Flujo AS-IS y Matriz de usuarios y necesidades | Abril Lara |
| #2 | Comparación de mecanismos e Indicadores de eficiencia | Cusme Vélez |
| #3 | Metáforas de interfaz y mapeo computacional | Gamboa Guamán |
| #4 | Prototipo interactivo navegable (Figma/Penpot) | Lozada Marcial |
| #5 | Protocolo de validación e Informe final | Martínez Jiménez |

**Regla:** un Issue se cierra solo cuando el entregable ya está subido al repo (no antes).

---

## 2. Commits

### Formato obligatorio

```
tipo(alcance): descripción breve en presente
```

**Tipos permitidos:**
| Tipo | Uso |
|---|---|
| `feat` | Agregar contenido/artefacto nuevo |
| `fix` | Corregir un error en un entregable |
| `docs` | Cambios en README o documentación |
| `refactor` | Reorganizar contenido sin cambiar su esencia |

### Ejemplos de commits significativos (correctos)

```
feat(diagnostico): agregar flujo AS-IS con tiempos muertos identificados
feat(mecanismos): completar matriz comparativa de 4 mecanismos evaluados
feat(metaforas): definir mapeo dominio-fuente a elemento digital
fix(prototipo): corregir enlace público de Figma sin permisos
docs(readme): actualizar tabla de integrantes y roles
```

### Ejemplos de commits que NO se aceptan

```
actualización
cambios
arreglo
subida de archivos
asdf
```

---

## 📌 3. Pull Requests

Solo se necesita **un PR** para todo el equipo (creado por un integrante, revisado por otro).

### Flujo recomendado

1. Trabajar en una rama propia: `feature/nombre-artefacto`
   ```bash
   git checkout -b feature/diagnostico-usuarios
   ```
2. Hacer commits siguiendo el formato de arriba.
3. Subir la rama:
   ```bash
   git push origin feature/diagnostico-usuarios
   ```
4. Abrir el Pull Request hacia `main`.
5. Otro integrante **revisa o comenta** el PR (no puede aprobar su propio trabajo).
6. Se integra (`merge`) a `main`.

### Plantilla para el Pull Request

```markdown
### Descripción
[Qué artefactos/carpetas incluye este PR]

### Issues relacionados
Closes #[número]

### Revisado por
@usuario-revisor

### Checklist
- [ ] El contenido corresponde al artefacto asignado
- [ ] Se mantiene coherencia con el flujo de gestión de citas
- [ ] Se respetan los principios de IHC (visibilidad, feedback, affordances)
- [ ] No hay archivos vacíos ni contenido de prueba
```

---

## 4. Buenas prácticas generales

- No hacer commits directos a `main` una vez creadas las ramas de trabajo.
- Cada carpeta numerada (`01-...` a `05-...`) pertenece a un responsable — evitar mezclar aportes ahí.
- Antes de cerrar un Issue, verificar que el entregable esté completo según la prueba práctica.
- Mantener el `README.md` actualizado con el estado de los Issues (`[ ]` / `[x]`).