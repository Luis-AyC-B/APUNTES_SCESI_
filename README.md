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