# Git Collaboration Lab 👋

¡Bienvenido al laboratorio de Git y GitHub!

Este repositorio es un pequeño ejercicio para aprender a colaborar en un proyecto de software utilizando **Git, ramas y Pull Requests**.

No necesitas experiencia previa con Git. Solo sigue los pasos.

## 🎯 Objetivo

Tu misión es agregar un saludo al programa `main.py` y enviarlo mediante un Pull Request.

El archivo inicialmente contiene:

```python
print("Hola, mundo!")
```

Al finalizar el ejercicio, debería contener saludos de diferentes integrantes:

```python
print("Hola, mundo!")
print("Hola, soy Ana")
print("Hola, soy Luis")
```

**Regla principal:** no modifiques directamente la rama `main`.

## 🛠️ Requisitos

Antes de comenzar, instala:

- [Git](https://git-scm.com/downloads)
- [Python](https://www.python.org/downloads/)
- [Visual Studio Code](https://code.visualstudio.com/) (recomendado)
- Una cuenta de [GitHub](https://github.com/)

Puedes verificar las instalaciones desde CMD:

```bat
git --version
python --version
```

## 🚀 Tutorial paso a paso

### 1. Clonar el repositorio

Abre CMD y ve a la carpeta donde quieras guardar el proyecto:

```bat
cd /d "D:\Proyectos"
```

Clona el repositorio:

```bat
git clone https://github.com/Zaffarone/git-collaboration-lab.git
```

Reemplaza `USUARIO` y `REPOSITORIO` por los datos reales del proyecto.

Entra a la carpeta:

```bat
cd git-collaboration-lab
```

### 2. Crear tu propia rama

Primero, asegúrate de tener la versión más reciente:

```bat
git switch main
git pull origin main
```

Ahora crea tu rama:

```bat
git switch -c feature/saludo-tu-nombre
```

Por ejemplo:

```bat
git switch -c feature/saludo-ana
```

Una rama permite trabajar en tus cambios sin modificar directamente la versión principal del proyecto.

### 3. Modificar el código

Abre el proyecto con VS Code:

```bat
code .
```

En `main.py`, agrega una línea con tu saludo:

```python
print("Hola, soy Ana")
```

No borres los saludos existentes.

Guarda el archivo con `Ctrl + S`.

Puedes ejecutar el programa con:

```bat
python main.py
```

### 4. Guardar tus cambios con Git

Primero, revisa qué modificaste:

```bat
git status
```

Agrega el archivo:

```bat
git add main.py
```

Crea un commit:

```bat
git commit -m "feat: add greeting from Ana"
```

Un *commit* registra una versión de tus cambios en el historial del proyecto.

### 5. Subir tu rama a GitHub

Ejecuta:

```bat
git push -u origin feature/saludo-ana
```

Utiliza el nombre real de tu rama.

¡Tu cambio ya está publicado en GitHub!

Todavía no está integrado en `main`.

### 6. Crear un Pull Request

Entra al repositorio en GitHub.

1. Abre la pestaña **Pull requests**.
2. Haz clic en **New pull request**.
3. Selecciona `main` como rama de destino (*base*).
4. Selecciona tu rama como origen (*compare*).
5. Escribe un título, por ejemplo: `Add greeting from Ana`.
6. Haz clic en **Create pull request**.

¡Terminaste tu parte del ejercicio!

La persona encargada del repositorio revisará tu Pull Request antes de integrarlo.

**No necesitas fusionarlo por tu cuenta.**

## ⚠️ ¿Qué pasa si aparece un conflicto?

Como todos modificaremos `main.py`, es posible que GitHub detecte conflictos entre algunos cambios.

¡Es normal!

Si aparece `This branch has conflicts that must be resolved`, no borres el trabajo de tus compañeros ni fuerces el merge. Comunícalo a la persona encargada para resolverlo juntos.

Parte del ejercicio consiste precisamente en aprender cómo colaborar cuando varias personas modifican el mismo proyecto.

## 📚 Comandos básicos

| Comando | Función |
|---|---|
| `git clone` | Descarga un repositorio |
| `git status` | Muestra el estado de los archivos |
| `git branch` | Muestra las ramas locales |
| `git switch -c` | Crea una rama y cambia a ella |
| `git add` | Prepara los cambios |
| `git commit` | Registra los cambios |
| `git push` | Sube commits a GitHub |
| `git pull` | Descarga e integra cambios remotos |

## ✅ Checklist de entrega

- [ ] Cloné el repositorio.
- [ ] Creé mi propia rama.
- [ ] Agregué mi saludo.
- [ ] Ejecuté el programa correctamente.
- [ ] Realicé un commit.
- [ ] Subí mi rama a GitHub.
- [ ] Creé mi Pull Request.
- [ ] Compartí el enlace del Pull Request con la coordinadora.

---

**¡Eso es todo!** 🎉

El objetivo no es escribir código complicado, sino aprender a colaborar de manera organizada.

*Un pequeño Hola Mundo, un gran paso hacia el trabajo en equipo.* 🚀
