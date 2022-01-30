# hello-world

Un repositorio para empezar a usar Github y Github Actions con Java

## ¿Como probar en el cloud?

[![](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/gitt-3-pat/hello-world)

# Práctica 1

## Comandos a probar

### Git clones

Se usa para copiar un repositorio de Git existente en un nuevo directorio local. De esta manera se creará un nuevo directorio local para el repositorio, se copiará todo el contenido del repositorio especificado y se creará las sucursales remotas rastreadas y extraerá una sucursal inicial localmente.

#### Logs:

``Cloning into 'hello-world'...
remote: Enumerating objects: 38, done.
remote: Counting objects: 100% (38/38), done.
remote: Compressing objects: 100% (23/23), done.
remote: Total 38 (delta 1), reused 31 (delta 0), pack-reused 0
Receiving objects: 100% (38/38), 58.97 KiB | 1.34 MiB/s, done.
Resolving deltas: 100% (1/1), done.``

### Git status
Permite mostrar el estado del directorio de trabajo y del área del entorno de ensayo. Se pueden ver los cambios que se han preparado y los archivos en los que Git no va a realizar el seguimiento.

#### Logs:

``On branch main
Your branch is up to date with 'origin/main'.``

``Changes to be committed:
(use "git restore --staged <file>..." to unstage)
deleted:    Practica1.txt``

``Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified:   README.md``

### Git add
Selecciona el archivo especificado y lo mueve al área de preparación, marcándolo para incluirlo en la próxima confirmación. Se puede seleccionar todos los archivos (.), un directorio, archivos específicos o incluso partes específicas de un archivo para preparar y confirmar

### Git commit
Guarda todos los cambios hechos en la zona de montaje o área de preparación (staging area), junto con una breve descripción del usuario.

#### Logs:

``Committer: Sergio Cuenca Núñez <sergiocuencanunez@MacBook-Pro-de-Sergio.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:``

    git config --global --edit

``After doing this, you may fix the identity used for this commit with:``

    git commit --amend --reset-author

``1 file changed, 167 insertions(+), 12 deletions(-)``

### Git push
Se usa para cargar contenido del repositorio local a un repositorio remoto. El envío es la forma de transferir confirmaciones desde el repositorio local a un repositorio remoto. Los envíos pueden sobrescribir los cambios, por lo que se debe tener cuidado a la hora de realizarlos.

#### Logs:

``Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 10 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 3.08 KiB | 3.08 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/SergioCuencaNunez/hello-world
1805845..df8af44  main -> main``

### Git checkout
Cambiar entre diferentes versiones de una entidad objetivo. Opera sobre tres entidades distintas: archivos, confirmaciones y ramas.

#### Logs:

``M       README.md
Your branch is up to date with 'origin/main'.``

## Evidencias de instalación del software

### Java 17

#### Logs:

``java version "17.0.1" 2021-10-19 LTS
Java(TM) SE Runtime Environment (build 17.0.1+12-LTS-39)
Java HotSpot(TM) 64-Bit Server VM (build 17.0.1+12-LTS-39, mixed mode, sharing)``

### Maven:

#### Logs:

``[INFO] Scanning for projects...
[INFO]
[INFO] ----------------------< com.mycompany.app:my-app >----------------------
[INFO] Building my-app 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.1.0:clean (default-clean) @ my-app ---
[INFO]
[INFO] --- maven-resources-plugin:3.0.2:resources (default-resources) @ my-app ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /Users/sergiocuencanunez/IdeaProjects/hello-world/src/main/resources
[INFO]
[INFO] --- maven-compiler-plugin:3.8.0:compile (default-compile) @ my-app ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /Users/sergiocuencanunez/IdeaProjects/hello-world/target/classes
[INFO]
[INFO] --- maven-resources-plugin:3.0.2:testResources (default-testResources) @ my-app ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /Users/sergiocuencanunez/IdeaProjects/hello-world/src/test/resources
[INFO]
[INFO] --- maven-compiler-plugin:3.8.0:testCompile (default-testCompile) @ my-app ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /Users/sergiocuencanunez/IdeaProjects/hello-world/target/test-classes
[INFO]
[INFO] --- maven-surefire-plugin:2.22.1:test (default-test) @ my-app ---
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit4/2.22.1/surefire-junit4-2.22.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit4/2.22.1/surefire-junit4-2.22.1.pom (3.1 kB at 6.2 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/2.22.1/surefire-providers-2.22.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-providers/2.22.1/surefire-providers-2.22.1.pom (2.5 kB at 48 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit4/2.22.1/surefire-junit4-2.22.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/surefire/surefire-junit4/2.22.1/surefire-junit4-2.22.1.jar (85 kB at 961 kB/s)
[INFO]
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running com.mycompany.app.AppTest
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.011 s - in com.mycompany.app.AppTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  1.943 s
[INFO] Finished at: 2022-01-21T19:55:32+01:00
[INFO] ------------------------------------------------------------------------ ``

## Comandos adicionales a probar

### Git branch
Ayuda a crear, eliminar y enumerar ramas. Las ramas son un puntero eficaz para las instantáneas de tus cambios. Cuando se quiere añadir una nueva función o solucionar un error, independientemente de su tamaño, se genera una nueva rama para alojar estos cambios.

#### Logs:

``* main``

### Git fetch
Se encarga de descargar commits, archivos y referencias de un repositorio remoto al repositorio local. Esta acción se lleva a cabo cuando se quiere ver en qué han estado trabajando los demás usuarios. Permite que la recuperación constituya una forma segura de revisar commits antes de integrarlos en tu repositorio local.

### Git merge
Permite tomar las líneas independientes de desarrollo creadas por git branch e integrarlas en una sola rama.

#### Logs:

``Already up to date.``

### Git pull
Se emplea para extraer y descargar contenido desde un repositorio remoto y actualizar al instante el repositorio local para reflejar ese contenido. Este comando es, en realidad, una combinación de dos comandos, git fetch seguido de git merge.

#### Logs:

``Already up to date.``

