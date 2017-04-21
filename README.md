# <img src="https://cdn4.iconfinder.com/data/icons/iconsimple-logotypes/512/github-256.png" width="40px" height="40px"/> Github - RoBorregos Workshop

Git es una herramineta o sistema útil para el manejo de versiones dentro de un proyecto. Github es una especie
de red socual basada en Git relacionado con el almacenamiento de proyectos y con el desarrollo colaborativo.
Github se caracteriza también por ser una herramienta y tener un servicio libre de paga, sin embargo, es posible
adquirir una cuenta con proyectos privados.

Sin embargo, así como Github nos puede ofrecer un enorme beneficio y ser un gran aliado de trabajo, también,
debido a un empleo no adecuado, puede terminar por revolver y crear un caos en nuestros proyectos.
Es debido a esto que se han establecido diferentes estándares de organización para el desarrollo con Github.

Dentro de este pequeño taller aprenderemos los conceptos básicos que se requieren para utilizar la herramienta
Github, así como uno de los estándares más utilizados a nivel profesional, para comenzar con la práctica instalaremos
github en nuestro equipo, posteriormente crearemos una cuenta en github, configuraremos nuestra cuenta para colaborar
en un proyecto, conoceremos los comandos en terminal para el trabajo colaborativo, realizaremos un ejercicio de
proyecto en equipo, hablaremos sobre una herramienta extra que nos facilitará aún más el trabajar en Github y
finalmente veremos los estándares que seguiremos dentro de la organización de RoBorregos en Github.


* conceptos básicos que se requieren para utilizar la herramienta Github
* uno de los estándares más utilizados a nivel profecional
* crearemos una cuenta en github
* configuraremos nuestra cuenta para colaborar en un proyecto
* conoceremos los comandos en terminal para el trabajo colaborativo
* realizaremos un ejercicio de proyecto en equipo
* hablaremos sobre una herramienta extra que nos facilitará aún más el trabajar en Github
* veremos los estándares que seguiremos dentro de la organización de RoBorregos en Github.

![git!=github](http://1.bp.blogspot.com/-WY2YpNr3W6g/UY6tZAc-H3I/AAAAAAAABLY/xJ9x3wIY8V8/s800/Github2.png)




## Conceptos.

* Repositorio
* Proyecto remoto
* Branch
* Commit
* Checkout
* Pull
* Push
* Pull request
* Fork
* Merge
* SSH key




## Estándar de branching.

Como se mencinó anteriormente, es sumamente importante el mantener un orden el en flujo de los commits, colaboraciones
al proyecto, para que nuestro trabajo no se vea afectado por cambios posteriormente y en caso de querer buscar algún segmento
en particular dentro del repositorio saber en qué versión estamos trabajando y dónde podemos encontrarlo, así como muchas
otras situaciones que se pudieran presentar.

Una de las distribuciones más populares dentro del área profesional es la que se le atribuye a la herramienta git flow,
de la cual hablaremos más adelante. Dicha organización se puede representar gráficamente de la siguiente forma:

<img src="http://nvie.com/img/git-model@2x.png" width="575px"></img>

### Branches principales

Dentro del modelo que emplearemos existen dos branches principales:
* master
* develop

enlistadas en orden de relevancia.

<img src="http://nvie.com/img/main-branches@2x.png" width="267px"></img>

### Branches auxiliares

A partir de las branches principales se desprenderán las branches auxiliares, dentro de las cuales se realizarán todos los
cambios al proyecto, es decir, las nuevas implementaciones dentro del proyecto o reparaciones de errores al mismo:
* features
* hotfixes

<img src="http://nvie.com/img/fb@2x.png" width="133px"></img>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="http://nvie.com/img/hotfix-branches@2x.png" width="316px"></img>

Si gustas leer y aprender más a fondo acerca de esta distribución te dejo el siguiente link al artículo fuente:

[A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)




## Instalación de Github.

#### Windows

Para instalar en un equipo con Windows deberás entrar a la siguiente liga para inciar la descarga y posteriomente la
instalación:

[Git para Windows](https://git-scm.com/download/win)

Dentro de las opciones de instalación les ofrecerá instalar Git Bash, lo cual es lo más recomendable, ya que será la
terminal que emplearemos para trabajar y comunicarnos con Github.


#### Linux

Ingresar los siguientes comandos en terminal:

```Shell
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
```


#### OSX

Ingresar los siguientes comandos en terminal:

```shell
$ brew install git
$ brew upgrade git
```

NOTA: En caso de no tener instalado Homebrew puedes entrar a la siguiente liga y seguir los pasos indicados.
[Homebrew](http://brew.sh/)




## Creación y configuración de usuario.

El primer paso será crear una cuenta personal en github. Una vez que se ha creado una seguirá el paso de la configuración
de nuestra cuenta con las credenciales o llaves necesarias para poder colaborar en un proyecto en equipo, para lo cual
seleccionaremos la opción **Settings** dentro del dropdown ubicado en la esquina superior derecha:

![Settings btn](./images/settings_btn.png)

Posteriormente, dentro del menú de opciones ubicado del lado izquierdo de la pantalla, daremos click en la opción **SSH and
GPG keys**:

![SSH and GPG keys btn](./images/ssh_gpg_btn.png)

Dentro de esta pantalla selecciona la opción de **New SSH key**:

![New SSH key](./images/new_ssh_btn.png)

Los pasos que debemos seguir para obtener la llave SSH de nuestro ordenador actual los podrás encontrar en el artículo
**[Generating a new SSH key and adding it to the ssh-agent](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)**.

Una vez generada la llave SSH le daremos un nombre en el campo de **Title** y pegaremos la llave dentro del campo **Key**.
Finalmente selecciona la opción de **Add SSH key**.

![Add SSH key](./images/add_ssh_key.png)




