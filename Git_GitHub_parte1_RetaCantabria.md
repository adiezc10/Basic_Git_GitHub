
# Curso Git + GitHub para Docentes - RETACantabria 2024/2025

## 1. Introducción a Git y GitHub
**Qué es Git**: Un sistema de control de versiones distribuido que permite registrar y gestionar cada cambio en los archivos de un proyecto. 

Permite gestión de versiones, ramificaciones, clonaciones y flujos de trabajo no lineales.

Sitio oficial: [git-scm.com](https://git-scm.com/)]

**Qué es GitHub**: Un servicio en la nube que aloja repositorios de código y facilita la colaboración en proyectos. Existen alternativas como GitLab y Bitbucket.

Sito oficial: [github.com/](https://github.com/)

Vídeo explicativo del funcionamiento de GitHub: [enlace](https://www.youtube.com/watch?v=w3jLJU7DT5E)

## 2. Instalación y configuración de Git
1. Descargar e instalar Git.

2. Verificar la instalación: Usa `git --version` en CMD para comprobar la versión instalada. Recomendaciones de actualización (versión 2.x en adelante).

3. Configuración inicial:

`git config --global user.name "Tu Nombre"`

`git config --global user.email "tu@correo.com"`

## 3. Registro y exploración de GitHub
### Crear una cuenta en GitHub. 
- [github.com/](https://github.com/)

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

## 4. Configuración y flujo de trabajo en Git

- Inicializar un repositorio: `git init`
- Clonar un repositorio existente: `git clone URL`
- Hacer cambios y confirmarlos: Añadir cambios al área de preparación: `git add`
- Confirmar cambios: `git commit -m "Descripción"`
- Flujo básico de Git: Sincronizar con un repositorio remoto: `git push` y `git pull`
- Gestión de ramas: Crear y cambiar ramas, merge, y resolución de conflictos.

## 5. Estrategias de control de versiones
GitFlow: Explicación de este flujo de trabajo.

## 6. Trabajar en proyectos Open Source
**¿Por qué contribuir?**: Visibilidad profesional y mejora de habilidades.

Dónde encontrar proyectos para contribuir:
- forgoodfirstissue
- goodfirstissue.dev
- goodfirstissues.com
Recomendaciones:
Seleccionar proyectos de interés personal.
Explorar cómo colaborar consultando el archivo CONTRIBUTING.md en cada repositorio.
Compartir logros: Cómo promocionar contribuciones en LinkedIn u otras redes profesionales.
## 7. Práctica Guiada
Crear y gestionar un repositorio: Ejercicio práctico de principio a fin.
Crear y gestionar ramas: Ejercicios con conflictos y merge.
Uso de Issues y Pull Requests: Simulación de un flujo de trabajo colaborativo.
## 8. Integraciones y Automatizaciones
GitHub Actions: Introducción a las automatizaciones en GitHub.
Otras integraciones útiles: Herramientas para mejorar la productividad (p. ej., Slack, Trello).
## 9. Buenas Prácticas y Consejos Finales
Documentación: Importancia de mantener un README claro y actual.
Commits claros y frecuentes: Ejemplos de buenos mensajes de commit.
Uso de .gitignore: Evitar subir archivos innecesarios.