# Tutorial Github
## ¿Qué es git?
-	Git es un software libre de control de versiones. Este tiene la capacidad de registrar las versiones de una gran cantidad de archivos del código fuente, manteniendo el registro de cambios en la propia computadora. También tiene la funcionalidad de fusionar código desde distintas computadoras, ya que provee herramientas específicas para fusionar código y evitar o manejar interferencias entre distintos códigos. 
## ¿Qué es GitHub?
-	GitHub es una plataforma en línea de desarrollo colaborativo que permite alojar proyectos utilizando Git.
## ¿Existen alternativas a GitHub?
-	Sí, dentro de las más famosas GitLab y BitBucket.
## ¿Por qué Github y no GitLab o BitBucket?
-	Es el más utilizado
-	Interfaz amigable y rápida
-	Provee wiki para documentar el proyecto
-	Seguimiento a los usuarios dentro del proyecto
-	Historial de modificaciones al código
-	Revisión de modificaciones al código
-	Reporte de errores en el código
-	Gran parte de sus funcionalidades son gratuitas, como repositorios públicos y privados, equipos de trabajo y manejo múltiples usuarios en un repositorio.
## ¿Qué beneficios tienen GitLab y BitBucket?
-	GitLab tiene una interfaz similar a GitHub
-	GitLab permite generar roles de usuario con permisos específicos, Github solo permisos de escritura y lectura a un repositorio.
-	GitLab tiene versión de código abierto, por lo tanto, se puede instalar en un servidor propio
-	BitBucket tiene integración nativa con herramientas como Trello y Slack
-	BitBucket tiene integración con Jira, software de la misma empresa que permite administrar tareas de un proyecto, hacer seguimiento de errores y la gestión operativa de este.
## ¿Cuáles son los precios?
-	Cada una tiene distintos valores, pero su principal limitacia es la posibilidad de hacer repositorios privados, cantidad de usuarios en equipos y cantidad de modificaciones que se le puede hacer a un código en un periodo de tiempo. Para el tamaño de nuestro equipo no tiene gran relevancia ya que las versiones gratuitas proveen todo lo que necesitamos. Las funcionalidades adquiridas en pagar son requeridas para equipos grandes o necesidades muy específicas. En caso de pagar, Bitbucket puede ser más conveniente en precios, pero con GitLab se puede integrar a un servidor propio y adquirir gran parte de las características de forma ilimitada.

# Terminología
Aquí se explicarán los términos más utilizados, para acceder a todos los términos utilizados dirigirse a [GitHub glossary](https://help.github.com/en/github/getting-started-with-github/github-glossary)
-	**Repository (repositorio):** El elemento más básico de GitHub, una especie de carpeta que contiene todo lo relacionado al proyecto y almacena cada archivo entre las diferentes versiones del código. Estos pueden tener múltiples colaboradores y ser públicos o privados.
-	**Branch (rama):** Versión paralela del repositorio que se encuentra dentro del mismo, esto permite seguir distintas líneas para el proyecto sin interferir entre sí. Se encuentra el Master Branch (rama maestra) que es donde se muestra la versión final del proyecto. Cada Branch se puede combinar para integrar los cambios de cada una en una versión final al Master Branch.
-	**Fork (bifurcación):** Copia personal de un repositorio en la cuenta propia. Permite utilizar el repositorio como se quiera, sin afectar de ninguna manera el original y manteniendo total control del repositorio.
-	**Clone (clonar):** Copia de un repositorio a la computadora. El repositorio local tiene un enlace a la versión en línea (GitHub), por lo tanto cuando se le indique puede realizar acciones en este.
-	**Pull (tirar):** Trae las actualizaciones de una rama del repositorio en línea y los mezcla con los archivos del computador local.
-	**Commit (comprometer):** Forma de formalizar un cambio en los archivos y registrarlos en git, aquí hablamos de un punto de guardado de una nueva versión del código. Esto solo hace referencia a los segmentos del código que han sido modificados. Por lo general llevan un comentario asociado para que al revisar el código se sepa que cambios se han hecho en esa versión.
-	**Push (empujar):** Actualiza los cambios realizados, y formalizados con commit, en la rama del repositorio local a la rama del repositorio en línea.
-	**Merge (mezclar):** Fusiona los cambios de una rama y los aplica en otro. Si un archivo no coincide con la versiones de la rama local, solicitará revisión del usuario para aprobar cual versión del código quedará.
-	**Status (estado):** Descripción del estado de la rama local del repositorio, indicando si falta hacer algún commit, problemas en el merge u otros.
-	**Add (añadir):** Analiza los archivos seleccionados para buscar cambios y los hace efectivos para el commit.
-	**Restore (restaurar):** Desecha todas las modificaciones en los archivos seleccionados a los que no se le ha realizado commit.

# Iniciar en Git y GitHub
## Instalar Git
Para Windows, descargar el instalador de [Download Git](https://git-scm.com/download/win) y hacer clic en instalar.
## Iniciar en GitHub
1.- Primero es necesario registrarse en [GitHub – Create your account](https://github.com/join?source=header). Recomiendo utilizar un correo personal ya que así la cuenta es personal y se registran las contribuciones que han hecho a los repositorios en los que participan, aunque sean privados. Les puede ser útil para mostrar su experiencia con git en otras empresas. Al tener los repositorios en una organización, si se desvincula a alguien perderá el acceso a los repositorios privados de la organización.
2.- Enviar el Username (nombre de usuario) para agregarlos a la organización de Bomberos de Chile.

# Uso de Git y vinculación con GitHub
Git se usa nativamente utilizando el termianl vía CMD o PowerShell para Windows. Algunos editores de texto permiten utilizar Git mediante su propia interfaz. Por ejemplo, Visual Studio Code tiene una sección para el controlador de versionamiento en su barra de herramientas lateral izquierda.<br>
![Vs Code Source Control](/images/vsc_source_control.png)<br>
Una vez vinculado con el repositorio el editor de texto da las facilidades para redactar mensajes en los commits y ejecutar comandos predeterminados.<br>
![Vs Code GitHub - Connected](/images/vsc_github_conected.png)<br>

## Iniciar repositorio Git local
Para iniciar un repositorio de forma local se hace con el comando <br><br>
`git init` <br><br>
el cual crea los archivos necesarios para el repositorio, en la carpeta .git (oculta por defecto por el explorador).

## Iniciar repositorio en GitHub (remoto)
En la barra lateral izquierda de la página inicial de GitHub se encuentra el botón New para añadir un nuevo repositorio<br>
![GitHub - New Repository](/images/github_new_repo.png)<br>
Aquí se permite seleccionar el Owner (dueño) del repositorio, si estas en una organización puedes crear un repositorio perteneciente a la organización. También se tiene que agregar nombre para el repositorio y una descripción (opcional). Se puede configurar si el repositorio es público o privado, en caso de ser público cualquier usuario puede ver el código que se encuentra y se puede administrar quienes pueden hacer commits, en el privado se tiene el manejo de quienes pueden acceder y hacer commits al repositorio.

Además se agrega la opción de agregar un README (leeme), archivo que se muestra al inicio del proyecto y es recomendado escribir descripción de los requerimientos para el proyecto y sus funcionalidades. Otras opciones adicionales son el .gitignore, que permite agregar en un archivo de texto los archivos o carpetas que no tienen que git debe ignorar, por lo que no serán subidas a github. Finalmente está el archivo de licencia, definidas para proyectos que pueden llegar al público e indica las condiciones en las que se puede utilizar el código.
![GitHub - Create New Repository](/images/github_create_new_repo.png)

## Enlazar/Subir un repositorio local a GitHub
Para enlazar/subir un repositorio local de git a GitHub es necesario crear el repositorio en GitHub como fue indicado anteriormente. Luego en la sección de Code (código) de repositorio, a la derecha se encuentra un botón verde que dice Clone or Download, el cual muestra un enlace. Luego abrimos el terminal en la carpeta de nuestro repositorio en git local e ingresamos el comando<br><br>
`git remote add origin enlace`<br><br>
![GitHub - Clone or Download Repository](/images/github_clone_download_repo.png)<br>

## Enlazar/Descargar un repositorio de Github al repositorio local
Crear el repositorio en GitHub y con el mismo enlace de la sección anterior ingresar el siguiente comando en la carpeta que quieres que se descargue el repositorio<br><br>
`git clone enlace`

## Efectuar cambios en el repositorio
Con el comando `git add` se efectúan cambios en el repositorio local, esto analiza los archivos que seleccionemos en búsqueda de archivos nuevos, eliminados y modificaciones. Esto prepara los archivos para el commit. Se puede realizar de distintas formas, los principales son:
-	Para efectuar todas las modificaciones, archivos nuevos y eliminados de la carpeta seleccionada por el terminal <br><br>
`git add -A`<br><br>
-	Para efectuar los cambios de un archivo/carpeta especifico <br><br>
`git add nombre-archivo`<br><br>
## Comprometer cambios en el repositorio
Para agregar las modificaciones efectuadas al repositorio local se utiliza el comando git commit y este puede contener un mensaje para especificar y dejar registro de qué cambios tiene esta versión del código, esto por medio del comando:<br><br>
`git commit –m “mensaje”`<br><br>
## Descargar modificaciones de github al repositorio local
Se descargan las modificaciones de la rama maestra de github al a la rama maestra del repositorio de local mediante el comando<br><br>
`git pull`<br><br>
este comando es una ejecución de un `git fetch`, que trae los archivos del repositorio remoto, seguido de un `git merge` que mezcla los archivos.
## Subir modificaciones del repositorio local a github
Se suben las modificaciones de la rama maestra del repositorio local a la rama maestra del repositorio de github mediante el comando<br><br>
`git push`<br><br>
Es recomendado hacer un `git pull` siempre antes de un `git push`<br><br>

## Mezclar repositororios
Cuando tenemos dos repositorios, ya sea local o remoto, se combinan estos. En ocaciones se puede editar código de un mismo archivo e incluso editar una misma linea. Esto genera un conflicto, ya que se tiene que decidir cual será el cambio que quedara finalmente. Aquí es donde Git tiene el comando <br><br>
`git merge`<br><br>
el cual combina los diferentes repositorios y cuando existe una interferencia se genera lo siguiente:<br><br>
   `<<<<<<< HEAD 
        <codigo local>
    >>>>>>>> 
     <codigo remoto>
     >>>>>>> 17ed5a8a2f2b44e4daf2302d63f6a6b8163xxxxx` <br><br>

aquí es donde quien se encuentra en el proceso de merge tiene que elegir qué código quedará finalmente, donde tiene que borrar todo y dejar solo el `<codigo>` que desea conservar. Luego se realiza un `git commit` para comprometer los cambios y un `git push`para subirlos al repositorio remoto.<br><br>
Recordar que el `git pull` incluye un `git merge`por lo que se realiza el mismo proceso al tener conflictos.
