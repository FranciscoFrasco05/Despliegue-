# Introducción a Git y Git Flow

## ¿Qué es Git?
Git es un sistema de control de versiones distribuido que permite a múltiples desarrolladores trabajar en un proyecto de manera simultánea. Algunas de sus principales características incluyen:

- **Rastreo de cambios**: Git guarda un historial completo de las modificaciones realizadas en un proyecto.
- **Colaboración**: Permite que múltiples desarrolladores trabajen en paralelo.
- **Ramas**: Ofrece la capacidad de trabajar en diferentes funcionalidades o fixes sin afectar el código principal.

## Comandos básicos de Git

### Configuración inicial
Antes de empezar, configura tu nombre y correo electrónico:
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"

Git Flow es una metodología que organiza el trabajo en ramas, facilitando la colaboración y el control de versiones. Se basa en el uso de ramas específicas:

Ramas principales
master/main:

Contiene el código listo para producción.
Solo se fusionan cambios estables.
develop:

Contiene el código en desarrollo.
Es la base para nuevas funcionalidades.
Ramas de soporte
feature:

Se crean para desarrollar nuevas funcionalidades.
Se basan en la rama develop.
release:

Se usan para preparar el código antes de su lanzamiento.
Permiten realizar pruebas y corregir errores.
hotfix:

Se usan para corregir errores críticos en producción.
Se basan en master y luego se fusionan tanto en master como en develop.
