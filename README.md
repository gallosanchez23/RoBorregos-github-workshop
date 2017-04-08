# <img src="https://cdn4.iconfinder.com/data/icons/iconsimple-logotypes/512/github-256.png" width="40px" height="40px"/> Github - RoBorregos Workshop

Git es una herramineta o sistema útil para el manejo de versiones dentro de un proyecto.
Github es el servisio de Git relacionado con el almacenamiento de proyectos y con el desarrollo colaborativo.
Github se caracteriza también por ser una herramienta y tener un servicio libre de paga, sin embargo,
es posible adquirir una cuenta con proyectos privados.

Sin embargo, así como Github nos puede ofrecer un enorme beneficio y ser un gran aliado de trabajo, también,
debido a un empleo no adecuado, puede terminar por revolver y crear un caos en nuestros proyectos.
Es debido a esto que se han establecido diferentes estándares de organización para el desarrollo con Github.

Dentro de este pequeño taller aprenderemos los conceptos básicos que se requieren para utilizar la herramienta
Github, así como uno de los estándares más utilizados a nivel profecional, posteriormente crearemos una cuenta
en github, configuraremos nuestra cuenta para colaborar en un proyecto, conoceremos los comandos en terminal para
el trabajo colaborativo, realizaremos un ejercicio de proyecto en equipo, hablaremos sobre una herramienta extra
que nos facilitará aún más el trabajar en Github y finalmente veremos los estándares que seguiremos dentro de la
organización de RoBorregos en Github.

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