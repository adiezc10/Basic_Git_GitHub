
# Introducción rápida a Git y GitHub

- [Introducción rápida a Git y GitHub](#introducción-rápida-a-git-y-github)
  - [1. Introducción a Git y GitHub](#1-introducción-a-git-y-github)
    - [Qué es Git](#qué-es-git)
    - [Qué es GitHub](#qué-es-github)
  - [2. Instalación y configuración de Git](#2-instalación-y-configuración-de-git)
  - [3. Registro y exploración de GitHub](#3-registro-y-exploración-de-github)
    - [Crear una cuenta en GitHub.](#crear-una-cuenta-en-github)
    - [Paseo por GitHub: principales herramientas](#paseo-por-github-principales-herramientas)
      - [Estructura de un repositorio en GitHub](#estructura-de-un-repositorio-en-github)
  - [4. Configuración y flujo de trabajo en Git](#4-configuración-y-flujo-de-trabajo-en-git)
  - [5. Estrategias de control de versiones](#5-estrategias-de-control-de-versiones)
    - [GitFlow](#gitflow)
    - [Otras estrategias](#otras-estrategias)
  - [6. Trabajar en proyectos Open Source](#6-trabajar-en-proyectos-open-source)
  - [7. Integraciones y Automatizaciones](#7-integraciones-y-automatizaciones)
  - [8. Buenas Prácticas y Consejos Finales](#8-buenas-prácticas-y-consejos-finales)
  - [9. Práctica guiada](#9-práctica-guiada)
  - [10. Markdown y VS Code](#10-markdown-y-vs-code)
    - [Qué es Markdown](#qué-es-markdown)
    - [Plugin recomendado: Markdown All in One](#plugin-recomendado-markdown-all-in-one)
      - [Características:](#características)
      - [Instalación:](#instalación)
      - [Uso básico:](#uso-básico)


---

## 1. Introducción a Git y GitHub

### Qué es Git
Git es un sistema de control de versiones distribuido que permite registrar y gestionar cada cambio en los archivos de un proyecto. Facilita la colaboración en equipos, ramificaciones, clonaciones y flujos de trabajo no lineales.  

- Sitio oficial: [git-scm.com](https://git-scm.com/)

### Qué es GitHub
GitHub es un servicio en la nube que aloja repositorios de código y facilita la colaboración en proyectos.  
Existen alternativas como GitLab y Bitbucket.

- Sitio oficial: [github.com](https://github.com/)
- Vídeo explicativo del funcionamiento de GitHub: [enlace](https://www.youtube.com/watch?v=w3jLJU7DT5E)

---

## 2. Instalación y configuración de Git
1. Descargar e instalar Git.

2. Verificar la instalación: Usa `git --version` en CMD para comprobar la versión instalada. Recomendaciones de actualización (versión 2.x en adelante).

3. Configuración inicial:

- `git config --global user.name "Tu Nombre"`
- `git config --global user.email "tu@correo.com"`

--- 

## 3. Registro y exploración de GitHub
### Crear una cuenta en GitHub. 
Registrarse en [github.com/](https://github.com/)

### Paseo por GitHub: principales herramientas

- **Home**: La página de inicio de GitHub, donde se muestran actualizaciones recientes de los repositorios que sigues, así como sugerencias de proyectos destacados.
    
    Aquí también puedes encontrar accesos directos a tus propios repositorios y notificaciones.

- **Issues**: Sistema de seguimiento de tareas, errores o mejoras propuestas dentro de un proyecto.
    
    - Tipos de Issues: Abiertos y cerrados, con posibilidad de etiquetarlos y asignarlos a miembros del proyecto.

    - Etiquetas: Organiza los issues con etiquetas que permiten priorizar y categorizar tareas, por ejemplo, bug, enhancement, o documentation.

- **Pull Requests** (PR):
Peticiones para fusionar cambios de una rama a otra. Son esenciales en la colaboración de proyectos, permitiendo revisión y discusión antes de integrar los cambios.
    - Flujo de una Pull Request: Crear una PR, revisar los cambios propuestos, discutir y sugerir mejoras, y finalmente aceptar o rechazar la fusión.
    - Revisiones y Comentarios: Es posible hacer revisiones de código, dejar comentarios específicos en líneas de código, y solicitar cambios adicionales.

- Projects: Herramienta para gestionar y planificar tareas del proyecto mediante tableros (similares a Trello/Planner).
    
    Tableros Kanban: Organiza las tareas en columnas como “Por hacer”, “En progreso” y “Completado” para facilitar la gestión visual de las tareas.

    Es ideal para seguir el progreso de un proyecto en equipo.

- **Discussions**: Espacio para conversaciones abiertas con la comunidad sobre temas diversos del proyecto, como ideas, preguntas, y feedback general.
    
    Es útil para interactuar con colaboradores sin necesidad de crear un issue o pull request.

- **Codespaces**: Entornos de desarrollo en la nube proporcionados por GitHub que permiten trabajar directamente desde el navegador. Configuración rápida, acceso desde cualquier lugar, y sincronización con el repositorio sin necesidad de configurar herramientas locales.

#### Estructura de un repositorio en GitHub
**Ejemplo práctico**: react de Meta/Facebook.

- Código: La sección principal donde se aloja el código fuente y otros archivos del proyecto.

- Vista de Archivos: Navega por los archivos y carpetas, explora ramas, y verifica el historial de commits.

- Ramas: Se gestionan las versiones del proyecto. La rama por defecto suele ser main, pero pueden existir otras para desarrollo o características específicas.

- Fork: Un fork es una copia del repositorio en tu cuenta de GitHub. Permite hacer cambios sin afectar el proyecto original. Una vez realizados los cambios, puedes proponer que se fusionen mediante una pull request.

- Starred: Marca un proyecto como favorito para facilitar su acceso y mostrar apoyo a los desarrolladores.
Las estrellas también sirven como un indicador de popularidad en la comunidad.

- Issues: Como se explicó anteriormente, es el lugar donde se rastrean y gestionan errores y sugerencias. Además, es un excelente punto de partida para quienes desean contribuir a proyectos open source buscando issues etiquetados como good first issue.

- Pull Request (PR): Aquí se encuentran las solicitudes de cambios que otros desean integrar en el proyecto. Puedes ver el historial de PRs, las discusiones sobre los cambios, y el estado (abierta, fusionada o cerrada).

---

## 4. Configuración y flujo de trabajo en Git

- Inicializar un repositorio: `git init`
- Clonar un repositorio existente: `git clone URL`
- Hacer cambios y confirmarlos: Añadir cambios al área de preparación: `git add`
- Confirmar cambios: `git commit -m "Descripción"`
- Flujo básico de Git: Sincronizar con un repositorio remoto: `git push` y `git pull`
- Gestión de ramas: Crear y cambiar ramas, merge, y resolución de conflictos.

---

## 5. Estrategias de control de versiones
### GitFlow
- **Ramas principales**: `main` y `develop`.
- **Ramas auxiliares**: `feature/*`, `release/*`, `hotfix/*`.
### Otras estrategias
- **Feature Branch Workflow**: Cada nueva funcionalidad en su propia rama.
- **Trunk-Based Development**: Realizar commits directamente en main.

--- 

## 6. Trabajar en proyectos Open Source
**¿Por qué contribuir?**
- Mejora tus habilidades técnicas.
- Visibilidad profesional.

Dónde encontrar proyectos para contribuir:
- [forgoodfirstissue](https://forgoodfirstissue.github.com/)
- [goodfirstissue.dev](https://goodfirstissue.dev/)
- [goodfirstissues.com](https://goodfirstissues.com/)


**Recomendaciones**: 
- Seleccionar proyectos de interés personal.
- Explorar cómo colaborar consultando el archivo `CONTRIBUTING.md` en cada repositorio.
- Compartir logros: Cómo promocionar contribuciones en LinkedIn u otras redes profesionales.

--- 

## 7. Integraciones y Automatizaciones
GitHub Actions: Introducción a las automatizaciones en GitHub.
Otras integraciones útiles: Herramientas para mejorar la productividad (p. ej., Slack, Trello).

---

## 8. Buenas Prácticas y Consejos Finales
Documentación: Importancia de mantener un README claro y actual.
Commits claros y frecuentes: Ejemplos de buenos mensajes de commit.
Uso de .gitignore: Evitar subir archivos innecesarios.

--- 

## 9. Práctica guiada
Crear y gestionar un repositorio: Ejercicio práctico de creación de apuntes con GitHub y GitHub Pages.

1. Creamos una carpeta en nuestro equipo, será nuestro repositorio.
2. Desde VScode creamos un archivo con extensión md.
3. Formateamos código con Markdown.
4. commit + pull
5. Comprobamos que el archivo está en github
6. Configuramos GitHub Pages: settings, code and automation, pages, branch = main

---
## 10. Markdown y VS Code
### Qué es Markdown
Markdown es un lenguaje de marcado ligero que permite crear documentos con formato de manera sencilla. Es ideal para README, blogs, documentación técnica, etc.

### Plugin recomendado: Markdown All in One
#### Características:
- **Previsualización en vivo**: Muestra cómo se verá el documento mientras lo editas.  
- **Atajos de teclado**: Facilita el formateo con comandos rápidos.  
- **Soporte para tablas, listas y encabezados**.  
- **Generación automática de índices (TOC)**: Crea índices dinámicos que se actualizan según los encabezados del documento.  

#### Instalación:
1. Abre VS Code.
2. Ve a la pestaña de extensiones (Ctrl+Shift+X).
3. Busca "Markdown All in One" e instálalo.
#### Uso básico:
- Previsualización: Ctrl+Shift+V.
- Generar una tabla de contenido automática: Inserta [TOC] en tu archivo.
- 