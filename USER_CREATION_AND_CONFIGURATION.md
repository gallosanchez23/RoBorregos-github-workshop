# Creación y configuración de usuario.

Primero que nada, para colaborar dentro de proyectos, crear nuestros propios repositorios o simplemente pertenecer a la comunidad de Github, es necesario generar una cuenta de usuario, la cual no tiene mayor ciencia que seleccionar la opción de **Sign Up** dentro de la página principal de [Github](https://github.com/) y llenar un formulario con tus datos personales.

<br>

> ***NOTA**: Los pasos que se describen a continuación, no son escenciales para trabajar con la Github, sin embargo, son convenientes y recomendados para trabajar de una forma más cómoda dentro de algún repositorio*

<br>

Una vez que ya poseas una cuenta de Github, podrás comenzar la fase de configuración de las credenciales requeridas para colaborar en repostorios ajenos. Esta configuración consiste básicamente en la generación de una clave pública [SSH](https://www.ssh.com/ssh/key/) (en caso de no tener ya una) y darla de alta en Github. La función de una clave pública SSH es similar a la de un nombre de usuario y contraseña: la autentificación de tu ordenador ante diferentes servicios automatizados, en este caso Github, con el fin de saber que eres tu quien está realizando cambios a un repositorio.

<br>

**1.** Para iniciar la configuración, selecciona la opción de **Settings** dentro del dropdown ubicado en la esquina suerior derecha, como se muestra a continuación.

![Settings btn](./images/settings_btn.png)

<br>

**2.** Posteriormente, dentro del menú de opciones ubicado en la parte izquierda de la pantalla, haz click en la opción de **SSH and GPG Keys**.

![SSH and GPG keys btn](./images/ssh_gpg_btn.png)

<br>

**3.** Dentro de esta pantalla selecciona la opción de **New SSH key**:

![New SSH key](./images/new_ssh_btn.png)

<br>

**4.** Deberás seguir los pasos descritos en el artículo **[Generating a new SSH key and adding it to the ssh-agent](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)** para generar la clave pública SSH de tu ordenador.

<br>

**5.** Ya que haz generado tu clave pública SSH deberás, ingresar en el campo **Title** un nombre con el cual puedas identificar el ordenador que la poseé, debido a que cada ordenador generará una SSH distinta. Finalmente copia y pega la clave pública SSH en el campo **Key** y selecciona la opcioón de **Add SSH key**

![Add SSH key](./images/add_ssh_key.png)

<br>

Con los pasos anteriores tu cuenta estará lista para colaborar en cualquier repositorio de Github, sin embargo, ahora será necesario realizar la **[Configuración de la terminal](TERMINAL_CONFIGURATION.md)**.
