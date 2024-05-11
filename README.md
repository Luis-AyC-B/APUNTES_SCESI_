# *CURSO GIT*
## Clase 1 :Introducción a Git
### CONCEPTO:
<span style="color:red">Este texto es rojo</span>
### <span style="color:red">CONCEPTO:</span>

Git es un sistema de control de versiones distribuido que facilita el seguimineto de cambios en archivos y la coordinacion del trabajo en equipo en proyectos de software.

[![5c9deef127c7d783462103.png](https://i.postimg.cc/SQtqmJYB/5c9deef127c7d783462103.png)](https://postimg.cc/23vgwjwG)

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

[![images.jpg](https://i.postimg.cc/NFVDfLV4/images.jpg)](https://postimg.cc/D4rLxf7J)

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

### Estrategias de fusión

[![git-merge-fusion-banner.png](https://i.postimg.cc/13yPrt4X/git-merge-fusion-banner.png)](https://postimg.cc/WhYQ2sGc)

- **Fusión Regular (Fast-forward)**: Git avanza la rama actual para fusionarla con la rama especificada si no hay conflictos.
- **Fusión de "Merge commit"**: Git crea un nuevo commit de fusión para combinar cambios, incluso si no hay conflictos.
- **Resolución de conflictos**: Cuando hay conflictos, Git requiere intervención manual para resolverlos antes de completar la fusión.

### Recursos adicionales
- [Documentación oficial de Git](https://git-scm.com/doc)
- [Tutorial de ramas en Git](https://www.atlassian.com/git/tutorials/using-branches)
- [Resolución de conflictos en Git](https://www.git-tower.com/learn/git/ebook/en/command-line/advanced-topics/merge-conflicts)

## Clase 3: GitHub

[![images.png](https://i.postimg.cc/rpFr3MZF/images.png)](https://postimg.cc/jDm2J0rG)

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

## Clase 4: Push, Pull y Pull Request

[![1676834249926.jpg](https://i.postimg.cc/wMxZstwY/1676834249926.jpg)](https://postimg.cc/MM4dCGk9)

### **Concepto básico**
El proceso de compartir y colaborar en proyectos Git involucra tres acciones fundamentales:

- **Push**: Este comando envía tus cambios locales al repositorio remoto, permitiendo que otros miembros del equipo accedan a tus contribuciones.
  
- **Pull**: Utilizado para obtener y fusionar los cambios desde el repositorio remoto a tu repositorio local, manteniendo tu copia del proyecto actualizada con la última versión.

- **Pull Request**: Una pull request es una propuesta de cambios que deseas integrar en el repositorio principal. Esta función es característica de plataformas de alojamiento de repositorios como GitHub, GitLab o Bitbucket. Facilita la revisión y discusión de cambios antes de fusionarlos en el repositorio principal.

### **Comandos**
- `git push`: Envía los cambios realizados en tu repositorio local al repositorio remoto.
  
- `git pull`: Obtiene los cambios del repositorio remoto y los fusiona automáticamente en tu repositorio local.
  
### **Flujo de trabajo sugerido**
1. **Crear una rama**: Antes de empezar a trabajar en una nueva funcionalidad, crea una rama nueva utilizando `git branch <nombre_rama>` y cámbiate a ella con `git checkout <nombre_rama>`.
  
2. **Realizar cambios**: Haz tus cambios en la rama creada y realiza commits regulares para mantener un historial claro de tus modificaciones.
  
3. **Sincronizar con el repositorio remoto**: Antes de enviar tus cambios, asegúrate de estar actualizado con el repositorio remoto utilizando `git pull`.
  
4. **Enviar tus cambios**: Utiliza `git push` para enviar tus cambios al repositorio remoto. Si estás trabajando en una rama diferente de la principal, puedes hacer un pull request para que tus cambios sean revisados antes de fusionarlos.
  
5. **Fusionar cambios**: Una vez que tus cambios han sido revisados y aprobados en el pull request, puedes fusionarlos en la rama principal utilizando la interfaz de la plataforma de alojamiento del repositorio o el comando `git merge`.

### **Extras**
- **Rebase**: Un método alternativo para integrar cambios que altera la historia de commits. Puede ser útil para mantener un historial de commits más limpio y lineal.
  
- **Squash**: Combina varios commits en uno solo, lo que puede ser útil para agrupar cambios relacionados y mantener un historial de commits más conciso.

## Clase 5: Gitflow

[![2-git-flow-model.png](https://i.postimg.cc/MHWHMDkZ/2-git-flow-model.png)](https://postimg.cc/xJ4nBLTB)

### Concepto básico
Gitflow es un flujo de trabajo para Git que define una estructura de ramas y reglas para facilitar el desarrollo colaborativo en proyectos de software. Propuesto por Vincent Driessen en 2010, Gitflow se ha convertido en un modelo popular para organizar el flujo de trabajo en equipos de desarrollo.

Gitflow se basa en la idea de tener dos ramas principales permanentes: `master` y `develop`. La rama `master` contiene el código estable y se utiliza para producir versiones de producción, mientras que la rama `develop` es la rama base para el desarrollo en curso. Además, Gitflow define varias ramas secundarias para características, versiones, hotfixes y lanzamientos.

### Ventajas de Gitflow
- **Claridad en el flujo de trabajo:** La estructura definida de ramas brinda una visión clara del progreso del desarrollo y el estado del código.
- **Separación de preocupaciones:** Las ramas separadas para características, hotfixes y versiones permiten trabajar en paralelo en diferentes aspectos del proyecto sin interferencias.
- **Facilidad para la colaboración:** Al seguir un modelo estandarizado, los equipos pueden colaborar de manera eficiente y predecible.

### Comandos comunes en Gitflow
Aunque no existen comandos específicos para Gitflow, su implementación implica el uso de varias operaciones comunes en Git:

- **Crear una nueva rama de función:** `git checkout -b feature/nombre_feature develop`
- **Iniciar un nuevo hotfix:** `git checkout -b hotfix/nombre_hotfix master`
- **Iniciar un nuevo release:** `git checkout -b release/1.0 develop`
- **Terminar una rama de función o hotfix:** `git merge --no-ff feature/nombre_feature` o `git merge --no-ff hotfix/nombre_hotfix`
- **Publicar una rama:** `git push origin nombre_rama`

### Integración con herramientas
Gitflow se integra bien con diversas herramientas y servicios, incluyendo:
- **Git Extensions:** Proporciona soporte gráfico para el flujo de trabajo de Gitflow.
- **GitKraken:** Ofrece una interfaz gráfica intuitiva que facilita la gestión de ramas y fusión según el modelo Gitflow.
- **GitHub Actions:** Permite automatizar flujos de trabajo basados en eventos, como despliegues automáticos después de la finalización de una rama de release.


> [!NOTE]
>Gitflow proporciona una estructura organizativa sólida y predecible para proyectos de desarrollo de software. Al seguir este modelo, los equipos pueden gestionar eficazmente el flujo de trabajo, colaborar de manera efectiva y entregar software de alta calidad de manera constante.

## Clase 6: Buenas Prácticas en Git

[![images-1.png](https://i.postimg.cc/Z5kkwqRp/images-1.png)](https://postimg.cc/hf03jcVt)

### Concepto básico
En esta clase aprenderemos sobre las prácticas recomendadas para el uso eficiente y seguro de Git. Estas prácticas son fundamentales para mantener la integridad y la colaboración en un proyecto de software. Algunas de estas prácticas incluyen:

> [!TIP]
> - **Escribir mensajes de commit claros:** Los mensajes de commit deben ser descriptivos y concisos, explicando de manera clara los cambios introducidos en el commit. Esto facilita la comprensión de los cambios realizados y su seguimiento en el historial del repositorio.
>
>- **Mantener ramas limpias:** Es importante mantener un número limitado de ramas en el repositorio y eliminar aquellas que ya no son necesarias. Las ramas deben tener nombres descriptivos y reflejar claramente su propósito, evitando ramas ambiguas o redundantes.
>
>- **Documentar cambios importantes:** Los cambios importantes en el código deben ser debidamente documentados, ya sea mediante comentarios en el código, actualizaciones en la documentación del proyecto o mediante registros en el sistema de seguimiento de problemas. Esto ayuda a mantener a todos los miembros del equipo informados sobre los cambios realizados y su impacto en el proyecto.

### Recomendaciones adicionales

> [!TIP]
> Algunas recomendaciones adicionales para mejorar la gestión de tu proyecto con Git:
>
>- **Utilizar branches por características:** En lugar de trabajar directamente en la rama principal del proyecto, considera crear branches separadas para cada nueva característica o corrección de errores. Esto facilita el seguimiento de los cambios y permite una mayor colaboración entre los miembros del equipo.
>
>- **Realizar revisión de código:** Antes de fusionar cambios en la rama principal, es recomendable realizar una revisión de código por parte de otros miembros del equipo. Esto ayuda a identificar posibles errores o mejoras en el código y garantiza la calidad del proyecto.
>
>- **Seguir convenciones de nomenclatura:** Establece convenciones de nomenclatura para los branches, commits y otros elementos del repositorio. Esto facilita la comprensión del proyecto y ayuda a mantener una estructura coherente en el repositorio.
>
>- **Automatizar tareas repetitivas:** Utiliza herramientas de automatización o scripts para realizar tareas repetitivas, como pruebas de integración, construcción de artefactos o despliegue de aplicaciones. Esto ahorra tiempo y reduce el riesgo de errores humanos.

### Implementación en VS Code

Puedes seguir estas prácticas en tu flujo de trabajo de Git directamente desde VS Code. Utiliza las extensiones disponibles en el marketplace de VS Code para mejorar la integración de Git en tu entorno de desarrollo. Algunas extensiones útiles incluyen:

- [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens): Proporciona una integración avanzada de Git en VS Code, permitiendo ver la autoría de líneas de código, historial de cambios, entre otros.

- [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph): Muestra un gráfico visual de las ramas y commits en tu repositorio, facilitando la comprensión de la estructura del proyecto.

- [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker): Ayuda a detectar errores de ortografía en tus mensajes de commit y comentarios de código.

Utiliza estas herramientas y prácticas recomendadas para mejorar tu flujo de trabajo con Git en VS Code y mantener tu proyecto de software organizado y eficiente

## Clase 7: Deshacer Cambios

### Concepto básico
En Git, es común cometer errores o necesitar deshacer cambios. Afortunadamente, Git ofrece varias formas de revertir cambios, resetear el estado de un archivo y manejar situaciones similares. Estas opciones permiten mantener el historial del proyecto limpio y corregir errores de manera eficiente.

> [!CAUTION]
> Estos comandos son destructivos y no destructivos

### Reset
El comando `git reset` permite deshacer cambios en el directorio de trabajo y el área de preparación. Tiene varias opciones que determinan el alcance del reset, como `--soft`, `--mixed` y `--hard`. Estas opciones determinan si los cambios deshechos se mantienen en el área de preparación o se eliminan por completo.

### Revert
Cuando necesitas deshacer los cambios introducidos por un commit anterior, puedes utilizar `git revert`. Este comando crea un nuevo commit que revierte los cambios introducidos por el commit especificado. Es útil cuando quieres mantener un historial limpio y no deseas reescribir la historia del repositorio.

### Eliminar commits
A veces, necesitas eliminar completamente un commit del historial. Puedes lograrlo utilizando comandos como `git reset --hard` o `git rebase -i`. Sin embargo, ten en cuenta que reescribir la historia del repositorio puede causar problemas si el repositorio es compartido con otros colaboradores.

## Comandos adicionales
Además de los comandos básicos, hay otras herramientas y técnicas que puedes utilizar para deshacer cambios en Git:

### Stash
El comando `git stash` guarda temporalmente los cambios locales sin hacer commit, lo que te permite trabajar en otra tarea. Puedes aplicar estos cambios posteriormente utilizando `git stash apply` o `git stash pop`.

### Cherry-pick
Cuando solo necesitas aplicar cambios específicos de un commit a tu rama actual, puedes utilizar `git cherry-pick`. Esto te permite seleccionar commits individuales y aplicarlos a tu rama actual.

### Reflog
El registro de referencia (`reflog`) registra los cambios en el puntero HEAD, lo que te permite recuperar fácilmente commits eliminados o perdidos. Puedes acceder al reflog utilizando `git reflog` y restaurar commits utilizando `git reset --hard HEAD@{<n>}`.

### Recomendaciones
- Antes de utilizar comandos que reescriben la historia del repositorio, asegúrate de entender las implicaciones y comunica tus acciones a los colaboradores del proyecto.
- Utiliza herramientas visuales como `gitk` o `git gui` para visualizar el historial del repositorio y comprender mejor los cambios realizados.

## Clase 8: Hooks, Alias y Trucos de Git

[![git-hooks-thumbnail.webp](https://i.postimg.cc/4NvCFgh0/git-hooks-thumbnail.webp)](https://postimg.cc/TpPHpB0j)

### Concepto básico:
Git ofrece características avanzadas que pueden mejorar significativamente la eficiencia y la automatización del flujo de trabajo. Algunas de estas características incluyen:

- **Hooks:** Son scripts que se ejecutan automáticamente en respuesta a ciertos eventos en Git, como pre-commit (antes de confirmar cambios) o post-merge (después de fusionar ramas). Los hooks permiten personalizar y automatizar tareas específicas del proyecto, como ejecutar pruebas unitarias o notificar a los miembros del equipo sobre cambios importantes.

- **Alias:** Los alias son atajos que permiten crear abreviaciones para comandos Git largos y frecuentemente utilizados. Por ejemplo, puedes crear un alias "st" para "git status" o "cm" para "git commit -m".

- **Varios trucos:** Además de los hooks y los alias, existen numerosos trucos y técnicas que los usuarios avanzados pueden emplear para optimizar su flujo de trabajo con Git. Estos trucos pueden incluir la combinación de comandos Git en secuencias eficientes, el uso de herramientas externas para complementar las funcionalidades de Git, o la integración de Git con otras herramientas de desarrollo.

### Comandos útiles:

- `git hooks`: Permite gestionar los hooks en un repositorio. Puedes agregar, eliminar o modificar los scripts de hook según las necesidades del proyecto.
  
- `git config --global alias.<nombre_alias> "<comando>"`: Crea un alias global para un comando de Git. Esto es útil para definir atajos personalizados que se aplicarán en todos los repositorios.

> [!IMPORTANT]
>Los comandos mencionados, los trucos específicos pueden variar según las necesidades del usuario y las particularidades del proyecto. Algunos ejemplos comunes incluyen la optimización de la configuración de Git, la automatización de tareas repetitivas mediante scripts personalizados, o el uso de extensiones de terceros para ampliar las capacidades de Git.
