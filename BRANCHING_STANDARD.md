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