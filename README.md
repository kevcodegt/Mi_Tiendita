# 🛒 Mi Tiendita

Sistema SaaS para la administración de pequeños y medianos negocios.

---

# 👥 Equipo de Desarrollo

| Integrante | Rol |
|------------|-----|
| Kevin Santizo | Arquitectura del sistema, UI/UX y Gestión del proyecto |
| Carlos Muñoz | Frontend |
| Emely Martín | Backend y Base de Datos |

---

# 🎯 Objetivo del Proyecto

Desarrollar un sistema SaaS moderno que permita administrar múltiples empresas, sucursales, inventario, ventas, clientes y reportes desde una única plataforma.

---

# 🛠 Tecnologías

## Frontend

- HTML5
- CSS3
- JavaScript
- React

## Backend

- Node.js
- Express.js

## Base de Datos

- PostgreSQL

## Control de Versiones

- Git
- GitHub
- Git Flow  https://git-flow-tutorial.readthedocs.io/en/feature-section-2/2-gitflow.html

---

# 📁 Estructura del Proyecto

```text
MiTiendita/
│
├── api/
├── assets/
├── backend/
├── database/
├── docs/
├── frontend/
├── README.md
└── .gitignore
```

---

# 🌳 Metodología de Trabajo

El proyecto utilizará **Git Flow**.

## Ramas

```text
main
develop
feature/*
release/*
hotfix/*
```

### Significado

| Rama | Descripción |
|------|-------------|
| `main` | Contiene el código estable listo para producción. |
| `develop` | Rama principal donde se integran todas las funcionalidades. |
| `feature/*` | Desarrollo de nuevas funcionalidades. |
| `release/*` | Preparación de una nueva versión para producción. |
| `hotfix/*` | Corrección de errores críticos encontrados en producción. |

---

# 💻 Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

- Git
- GitHub CLI (Opcional)
- Homebrew (macOS)
- Git Flow

---

# 🍺 Instalar Homebrew (macOS)

Verificar instalación:

```bash
brew --version
```

Si no está instalado:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

---

# 🧰 Instalar Git

Verificar:

```bash
git --version
```

---

# 🌿 Instalar Git Flow

Instalar:

```bash
brew install git-flow
```

Verificar:

```bash
git flow version
```

---

# 🚀 Clonar el Proyecto

Por SSH:

```bash
git clone git@github.com:kevcodegt/Mi_Tiendita.git
```

Entrar al proyecto:

```bash
cd Mi_Tiendita
```

---

# ⚙ Inicializar Git Flow

Ejecutar una sola vez dentro del proyecto:

```bash
git flow init
```

Aceptar la configuración predeterminada:

```text
Production branch: main
Development branch: develop

Feature prefix: feature/
Bugfix prefix: bugfix/
Release prefix: release/
Hotfix prefix: hotfix/
Support prefix: support/
Version tag prefix: v
```

---

# 🌱 Flujo de Trabajo

## 1. Actualizar la rama de desarrollo

```bash
git checkout develop
git pull origin develop
```

---

## 2. Crear una nueva funcionalidad

```bash
git flow feature start login
```

Esto creará automáticamente la rama:

```text
feature/login
```

---

## 3. Guardar cambios

```bash
git add .
git commit -m "feat: agregar pantalla de login"
```

---

## 4. Finalizar la funcionalidad

```bash
git flow feature finish login
```

Git Flow realizará el merge automáticamente hacia `develop`.

---

## 5. Subir cambios

```bash
git push origin develop
```

---

# 📦 Comandos Git Más Utilizados

Ver estado:

```bash
git status
```

Ver ramas:

```bash
git branch
```

Ver todas las ramas:

```bash
git branch -a
```

Cambiar de rama:

```bash
git checkout nombre-rama
```

Actualizar repositorio:

```bash
git pull
```

Subir cambios:

```bash
git push
```

Historial:

```bash
git log --oneline --graph --all
```

Ver diferencias:

```bash
git diff
```

---

# 📌 Convención de Commits

Utiliza mensajes claros y descriptivos.

| Tipo | Ejemplo |
|------|----------|
| feat | `feat: agregar módulo de productos` |
| fix | `fix: corregir validación de login` |
| docs | `docs: actualizar README` |
| style | `style: mejorar interfaz del dashboard` |
| refactor | `refactor: reorganizar estructura del backend` |
| chore | `chore: actualizar dependencias` |

---

# 📋 Reglas del Equipo

- Nunca trabajar directamente sobre `main`.
- Todas las funcionalidades deben desarrollarse desde `develop`.
- Cada tarea debe tener su propia rama `feature/*`.
- Realizar commits pequeños y frecuentes.
- Antes de comenzar una tarea, actualizar `develop`.
- Resolver conflictos antes de realizar un merge.
- Mantener el código limpio y documentado.
- Todo cambio debe quedar registrado mediante commits descriptivos.

---

# 📚 Documentación

Toda la documentación del proyecto deberá almacenarse en:

```text
docs/
```

---

# 📄 Licencia

Proyecto académico desarrollado por el equipo **Mi Tiendita**.
