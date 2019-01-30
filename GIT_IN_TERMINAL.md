## Git en terminal.

Primeramente conoceremos los comandos para configurar nuestra cuenta de Github en terminal:

```shell
$ git config --global user.name 'Nombre y apellido'
$ git config --global user.email 'email@roborregos.mx'
```

Una vez que nos hayamos presentado con Git por medio de nuestra terminal, primeramente conoceremos los comandos básicos
para las acciones relacionadas con iniciar un repositorio desde cero, branching y el manejo de versiones dentro del repositorio
y posteriormente comandos que nos facilitarán la colaboración de varios miembros de un equipo dentro de dicho repositorio.


#### Inicializar un repositorio

Para empezar un repositorio dentro de github vamos a trabajar tanto en terminal como en el navegador. El primer paso para
esto será entrar en nuestro navegador al sitio oficial de **[github](https://github.com)** y dar click sobre el botón de nuevo
repositorio:
![New Repository Button](./images/new_repository_btn.png)

Este botón nos llevará a la pantalla de creación de un repositorio nuevo, donde elegiremos el nombre, insertaremos la descripción
y decidiremos si queremos que nuestro repositorio sea público o provado. Finalmente, la última sección de esta vista nos ofrece la
opción de inicializar el repositorio con un archivo README o sin él. Existen dos opciones para crear un repositorio nuevo, enlazar
un proyecto existente en alguna carpeta local, o inicializar un repositorio vacío en donde posteriormente crearemos un nuevo proyecto.
Para la primera opción en la que enlazaremos un proyecto local existente, no se debe seleccionar el checkbox, es decir que no
inicializaremos nuestro repositorio con un README. En caso de no querer enlazar un proyecto local con el nuevo repositorio, es
recomendable seleccionar la opción de inicializar el repositorio con un README, de esta forma se creará un repositorio listo para ser
clonado.


#### Enlazar un proyecto existente

Una vez creado nuestro reposotiro dentro de github sin un README, el siguiente paso será enlazar un proyecto local con el repositorio
ya existente. Para esto, el primer paso que debemos realizar es ubicarnos en el directorio del proyecto desde la terminal y
utilizaremos los siguientes comandos.

```shell
$ git init
```
para inicializar el directorio como un proyecto de git.

```shell
$ git add .
$ git commit -m 'Initial commit'
```
para agregar todos los archivos existentes en el proyecto a un commit inicial.

```shell
$ git remote add origin "repository_URL"
```
para agregar el enlace entre el repositorio creado en github y el directorio local del proyecto previamente inicializado en git.
Sustituye "repository_URL" con el url proporcionado por tu repositorio, ya sea SSH o HTTPS.

```shell
$ git push -u origin master
```
para finalmente subir los archivos de tu proyecto local al repositorio.


#### Clonar un repositorio

En caso de tener un repositorio existente con un proyecto en el que se quiere trabajar, será necesario crear una copia local en la
cual poder seguir con el desarrollo y posteriormente subir los cambios realizados al repositorio, para lo que requeriremos "clonar"
el proyecto, lo cual no es complicado de realizar. El primer paso será colocarte por medio de la terminal en el directorio donde se
desea guardar el proyecto, y posteriormente ingresar el siguiente comando que simplemente clonará el proyecto dentro del repositorio
deseado

```shell
$ git clone "repository_URL"
```
en donde "repository_URL" será el url SSH proporcionado por tu repositorio.


#### Branching

Una vez que se tiene el proyecto clonado en un direcotio local, estamos listos para comenzar a trabajar en él. Para ello, una de las
principales ventajas y herramientas que nos ofrece Github que podemos aprovechar es una de la que ya hablamos: el branching, o en
español: las derivaciones o ramificaciones.
A continuación se muestran los comandos para el empleo y manipulación de branches dentro de un proyecto con git.

Muestra las branches existentes en tu proyecto local y saber en la que te encuentras actualmente:
```shell
$ git branch
```

Permite visualizar las branches que existen tanto remota como localmente:
```shell
$ gith branch -r
```

Útil para cambiar de branch en la que nos encontramos:
```shell
$ git checkout "branch_name"
```

Para crear una nueva branch local, cambiarte a ella y posteriormente subirla al repositorio:
```shell
$ git branch "new_branch_name"
$ git checkout "new_branch_name"
$ git push origin "new_branch_name"
```

En caso de querer eliminar una branch en tu proyecto local:
```shell
$ git branch -d "branch_name"
```

En caso de querer eliminar una branch tanto en tu proyecto local como en el repositorio:
```shell
$ git push origin --delete "branch_name"
```

Una vez que se ha terminado de desarrollar dentro de una branch o se ha cumplido el objetivo de esa branch, es hora de unirla a la
branch de donde surgió ésta, para lo cual utilizaremos el comando:
```shell
$ git merge "branch_name"
```
Cuando este comando sea ejecutado, la branch "branch_name" será unida a la última versión de la branch de la que surgió, con la
excepción de los casos en los que exista conflictos en algún documento en el que se hayan efectuado cambios.


#### Trabajo colaborativo

Para este punto, tu ya sabes que github es una red socual para colaborar en proyectos con tus amigos y compañeros de trabajo, así como
que es diferente el proyecto que tienes localmente en tu ordenador y el proyecto que se encuentra en el repositorio en la web, ya que
al momento de que tu realizas cambios en los archivos, los realizarás solo localmente, para lo que posteriormente será necesario
subirlos al repositorio, y así tus demás compañeros podrán descargarlos a sus proyectos locales. De esta forma, todos pueden trabajar
con los cambios que los demás integrantes del equipo realizan en el proyecto. De esta forma, git adopta una modalidad de manejo de
versiones en el repositorio en el que se trabaja, permitiendo que, siendo empleado de la forma adecuada, los colaboradores trabajen
con las versiones más actualizadas de los proyectos.

Ahora bien, una vez que conocemos la forma en la que trabaja git, es momento de conocer cómo trabajar con él de la forma óptima utilizando
los comandos adecuados.
Primero que nada, es importante siempre que nos vayamos a centar a trabajar, saber que estamos trabajando con la versión más actualizada
en la branch actual con los cambios que todos los integrantes del equipo hayan realizado. Para esto es importante siempre que iniciemos
descargar los cambios nuevos que existan en el repositorio, para lo que utilizaremos el siguiente comando:
```shell
$ git pull origin "branch_name"
```
sustituyendo "branch_name" por el nombre de la branch en la que nos encontramos. Posterior a este comando podremos trabajar y modificar los
documentos más actualizados en el proyecto.

Una vez que hayamos comenzado a trabajar en nuestro proyecto local, podemos berificar los archivos que hayamos editado desde el último push
o la última actualización que hayamos realizado en el repositorio. Para esto podemos utilizar el comando
```shell
$ git status
```
Es importante mencionar también que este comando no solo nos muestra los archivos que hayamos editado localmente, sino que también nos
genera un informe completo sobre la branch en la que nos encontramos actualmente, si nos hace falta realizar un pull del repositorio
y clasifica los cambios que hemos realizado entre cambios sin preparar para un commit y cambios listos dentro de un commit, remarcándolos
con colores rojo y verde.
