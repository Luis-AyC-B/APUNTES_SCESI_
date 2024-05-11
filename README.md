# *CURSO GIT*
## Clase 1 :Introducción a Git
### CONCEPTO:
Git es un sistema de control de versiones distribuido que facilita el seguimineto de cambios en archivos y la coordinacion del trabajo en equipo en proyectos de software.

### Comandos:
- `git init`: En un directorio inicializa el repositorio Git.
- `git add <archivo>`: Agrega un archivo a nuestra área de preparación.
- `git commit -m "Mensaje"`: Nos ayuda a guardar  los cambios en un repositorio (punto de guardado).

## States y Commits
### Concepto básico:

- *Directorio de trabajo:* Es el espacio donde trabajamos con nuestros archivos y se realiza cambios.
- *Área de preparación (Staging Area):* Es donde seleccionas los cambios que quieres incluir en tu próximo commit.
- *Repositorio:* Es un almacenamiento virtual de tu proyecto. Te permite guardar versiones del código a las que puedes acceder cuando lo necesites.

### Comandos:

- `git status`:  Muestra el estado del directorio de trabajo y del área del entorno de ensayo.
- `git log`: Muestra el historial de commits. Proporciona una lista detallada de todos los commits realizados en el repositorio, incluyendo el autor, la fecha y el mensaje asociado a cada commit.
- `git diff`: Muestra las diferencias entre versiones. Puedes usar este comando para ver las diferencias entre el directorio de trabajo y el área de preparación, entre el área de preparación y el último commit, o entre dos commits específicos.

## Clase 2: Ramas, Merge y Conflictos

### Concepto básico
Las ramas en Git permiten trabajar en paralelo en diferentes funcionalidades o correcciones de errores. Cada rama representa una línea independiente de desarrollo. Merge combina cambios de diferentes ramas, y los conflictos ocurren cuando hay cambios contradictorios que deben resolverse manualmente.

### Comandos
- `git branch <nombre_rama>`: Crea una nueva rama con el nombre especificado.
- `git checkout <nombre_rama>`: Cambia a una rama específica.
- `git merge <nombre_rama>`: Combina los cambios de una rama en otra. Esto fusiona los cambios de la rama especificada en la rama actual. Si hay conflictos, Git pausará el proceso de fusión y requerirá que los resuelvas manualmente.

### Uso avanzado
- `git branch -d <nombre_rama>`: Elimina una rama después de que sus cambios se han fusionado correctamente en otra rama.
- `git branch -D <nombre_rama>`: Elimina una rama incluso si sus cambios no se han fusionado en otra rama (se pierden los cambios no fusionados).
- `git merge --abort`: Cancela el proceso de fusión en caso de conflicto y restaura el estado antes de la fusión.
- `git merge --no-ff <nombre_rama>`: Realiza un merge "no fast-forward", creando un nuevo commit de merge incluso si Git podría hacerlo automáticamente.

### Uso avanzado
- `git branch -d <nombre_rama>`: Elimina una rama después de que sus cambios se han fusionado correctamente en otra rama.
- `git branch -D <nombre_rama>`: Elimina una rama incluso si sus cambios no se han fusionado en otra rama (se pierden los cambios no fusionados).
- `git merge --abort`: Cancela el proceso de fusión en caso de conflicto y restaura el estado antes de la fusión.
- `git merge --no-ff <nombre_rama>`: Realiza un merge "no fast-forward", creando un nuevo commit de merge incluso si Git podría hacerlo automáticamente.

### Estrategias de fusión
- **Fusión Regular (Fast-forward)**: Git avanza la rama actual para fusionarla con la rama especificada si no hay conflictos.
- **Fusión de "Merge commit"**: Git crea un nuevo commit de fusión para combinar cambios, incluso si no hay conflictos.
- **Resolución de conflictos**: Cuando hay conflictos, Git requiere intervención manual para resolverlos antes de completar la fusión.

### Recursos adicionales
- [Documentación oficial de Git](https://git-scm.com/doc)
- [Tutorial de ramas en Git](https://www.atlassian.com/git/tutorials/using-branches)
- [Resolución de conflictos en Git](https://www.git-tower.com/learn/git/ebook/en/command-line/advanced-topics/merge-conflicts)

## Clase 3: GitHub

### Concepto básico
GitHub es una plataforma de alojamiento de repositorios Git en la nube, que facilita la colaboración en proyectos de código abierto y privados. Permite a los desarrolladores trabajar juntos en proyectos de software, gestionar versiones de código, realizar seguimiento de problemas y solicitar características nuevas, todo de forma colaborativa.

Además de alojar repositorios Git, GitHub ofrece una variedad de herramientas y servicios adicionales, como integración continua, seguimiento de problemas, wikis de proyectos y soporte para documentación técnica.

### Crear un repositorio en GitHub
Una de las tareas básicas en GitHub es la creación de un nuevo repositorio. Este proceso se puede realizar de la siguiente manera:

1. Inicia sesión en tu cuenta de GitHub.
2. En la esquina superior derecha de la página, haz clic en el botón "+" y selecciona "Nuevo repositorio".
3. Completa el nombre y la descripción de tu repositorio, así como otras opciones como la visibilidad (público o privado) y el archivo README.
4. Haz clic en el botón "Crear repositorio".

### Otras funcionalidades de GitHub
Además de alojar repositorios, GitHub ofrece una amplia gama de funcionalidades que pueden mejorar la colaboración y la gestión de proyectos:

- **Seguimiento de problemas:** GitHub proporciona un sistema de seguimiento de problemas que permite a los usuarios reportar errores, solicitar características y discutir ideas.
- **Pull requests:** Los pull requests son solicitudes para incluir cambios en un repositorio. Permiten a los colaboradores revisar, comentar y aprobar los cambios propuestos antes de fusionarlos con la rama principal del proyecto.
- **Integración continua:** GitHub Actions permite automatizar flujos de trabajo, como pruebas unitarias, construcción de proyectos y despliegue, directamente desde el repositorio de GitHub.
- **Wikis de proyectos:** GitHub ofrece la posibilidad de crear wikis para documentar el proyecto, proporcionando un espacio para compartir información sobre la arquitectura, las mejores prácticas y los procesos de desarrollo.
- **Gestión de proyectos:** GitHub Projects permite crear tableros kanban para organizar y priorizar tareas, así como realizar un seguimiento del progreso del proyecto.

### Comandos útiles de Git para trabajar con GitHub
Aunque GitHub es una plataforma en sí misma, se utiliza en conjunto con Git para gestionar repositorios. Algunos comandos útiles de Git para trabajar con GitHub incluyen:

- `git clone <url_del_repositorio>`: Clona un repositorio de GitHub en tu máquina local.
- `git remote add origin <url_del_repositorio>`: Conecta un repositorio local a un repositorio remoto en GitHub.
- `git push origin <nombre_rama>`: Envía los cambios de una rama local a un repositorio remoto en GitHub.
- `git pull origin <nombre_rama>`: Obtiene los cambios de un repositorio remoto en GitHub y los fusiona con la rama local.