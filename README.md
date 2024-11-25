# Git y Git Flow

## ¿Qué es Git?
Git es un sistema de control de versiones distribuido diseñado para rastrear los cambios en el código fuente durante el desarrollo de software. Fue creado por **Linus Torvalds** en 2005 y se utiliza ampliamente para gestionar proyectos pequeños y grandes de manera eficiente.

### Principales características de Git:
- **Distribuido**: Cada desarrollador tiene una copia completa del historial del proyecto.
- **Versionado**: Permite mantener un historial de los cambios realizados en el código.
- **Colaboración**: Facilita el trabajo en equipo al permitir fusionar los cambios de diferentes colaboradores.
- **Velocidad**: Optimizado para operaciones rápidas como commits, branch y merges.

---

## ¿Qué es Git Flow?
Git Flow es un modelo de flujo de trabajo basado en Git que define una estructura clara para gestionar ramas en un proyecto. Fue propuesto por **Vincent Driessen** y es popular por su enfoque lógico y organizado.

### Principales ramas en Git Flow:
1. **master**:
   - Contiene el código en producción.
   - Siempre debe estar estable.

2. **develop**:
   - Es la rama principal para el desarrollo.
   - Contiene el código que se fusionará en la rama `master` después de ser probado.

### Ramas de soporte:
- **feature**:
  - Se crean desde `develop` para implementar nuevas funcionalidades.
  - Se fusionan de nuevo en `develop`.

- **release**:
  - Se crean desde `develop` cuando se prepara una nueva versión para producción.
  - Se fusionan en `master` y `develop`.

- **hotfix**:
  - Se crean desde `master` para corregir errores críticos en producción.
  - Se fusionan en `master` y `develop`.

### Flujo de trabajo básico:
1. Crear una nueva rama `feature` para una funcionalidad específica.
2. Finalizar la funcionalidad y fusionar la rama `feature` en `develop`.
3. Crear una rama `release` cuando se vaya a preparar una nueva versión.
4. Fusionar `release` en `master` y etiquetarla con un número de versión.
5. Usar ramas `hotfix` para corregir problemas urgentes.

### Ventajas de Git Flow:
- Estructura clara y bien definida para ramas.
- Facilita la gestión de proyectos complejos con múltiples desarrolladores.
- Compatible con procesos de entrega continua y control de versiones.

---

## Resumen
Git es la herramienta de control de versiones, mientras que Git Flow es un modelo de trabajo que organiza el uso de ramas dentro de Git para un desarrollo eficiente y ordenado.

