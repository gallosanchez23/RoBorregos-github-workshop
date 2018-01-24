# Conceptos básicos.

#### Repositorio.
La forma más fácil de imaginar un repositorio es como un directorio en el que se encuentran alojados archivos y directorios a la medida del proyecto. Dentro de un repositorio es donde se realizan todas las acciones concernientes al proyecto correspondiente, tales como generar **branches**, realizar **forks**, **merges**, entre otras acciones.

#### Proyecto remoto.
Se refiere a un proyecto alojado en algún servidor, en este caso de Github, el cual puede ser consultado y modificado, entre otras acciones. La gran ventaja que un proyecto remoto ofrece es el hecho de poder consultarlo desde cualquier lugar físico, al igual que abre las puertas a una libre colaboración por parte de diferentes miembros de un equipo,

#### Branch.
Es una versión paralela del repositorio que te permite trabajar sin preocupación alguna de modificar indebidamente la versión principal. Una vez que los cambios han sido probados y declarados como funcionales o correctos, se puede hacer un **merge** a la **branch** principal. Las **branches** son las que le permiten a Git un manejo de versiones tan eficiente.

#### Commit.
Se refiere a la agrupación de cambios en uno o más archivos del repositorio. Para cada **commit** Github crea un ID único, permitiendo al usuario redactar un breve mensaje descriptivo acerca de los cambios que se agrupan en él, y al momento de realizar **push** al repositorio, conocer el colaborador que realizó este **commit**.

#### Checkout.
Un **checkout** tiene dos principales funciones, el manejo de **branches**, al permitirnos crear y cambiarnos de una a otra, y el borrar los cambios o restablecer los archivos deseados al úlimo **pull** o **push** realizado sobre los mismos. Básicamente es decirle a Github a dónde queremos que voltee a ver.

#### Pull.
Es la acción de bajar los cambios realizados en el repositorio remoto y actualizar una **branch** local. También es posible realizar **pull** de **commits** locales, de forma que se genera un **merge**. Realizar **pull** te permite estar actualizado con respecto a los cambios generados en el repositorio, por lo que es muy recomendado realizarlos periódicamente y siempre antes de realizar un **push**.

#### Push.
Es la acción de publicar o subir al repositorio remoto los **commits** realizados localmente hasta el momento. De esta forma, los demás colabradores del proyecto podrán ver tus cambios y realizar un **pull** de los mismos.

#### Pull request.
Se refiere a la propuesta de cambio para una branch dentro de un repositorio. A diferencia de un **push** o un **merge**, el **pull request**, su objetivo es que puede ser revisado, comentado, modificado y aceptado por otro colaborador del repositorio, de modo que los cambios sean discutidos y finalmente realizar el **merge** propuesto.
	
#### Clone.
Es un comando o acción que te permite generar una **copia local** en tu ordenador de un repositorio remoto alojado en Github.

#### Fork.
Es una acción que genera una copia remota de un repositorio remoto alojado en Github, es decir que se creará un repositorio exactamente igual que el deseado. A diferencia del **clone**, el cual implica una copia local, el **fork** genera una copia remota (en Github), no local (en tu ordenador). Realizar un **fork** no afecta el proyecto original.

#### Merge.
Se refiere al proceso de tomar los cambios de una **branch** y unirlos con otra. Al realizar un **merge**, se toma el último **commit** de la “Branch Origen” y se empatan los cambios realizados con respecto a la "Branch Destino". Un **merge** no modifica la “Branch Origen”.

#### Conflictos.
Surgen al momento de querer realizar un **merge** a dos branches que han sido modificadas de forma independiente en los mismos archivos, por lo que Github no sabrá con cual de las dos versiones quedarse.

#### SSH key.
La función de una clave pública **SSH** (SSH key) es similar a la de un nombre de usuario y contraseña: la autentificación de tu ordenador ante diferentes servicios automatizados, en este caso Github.

<br>

Los conceptos anteriores son los que consideramos básicos para comenzar a trabajar con Git y Github. En caso de que te interece conocer más a fondo estos y más conceptos concernientes te sugerimos leer el [Glosario de Github](https://help.github.com/articles/github-glossary/).