<img src='./assets/Enlazando.png'>


## Enlazando nuestro primer Repo

Ya tenemos por un lado el repo de las carpetas con su control de versiones, pero nos falta asignarlo a un repo de GitHub. Para esto haremos lo siguiente:

1. Iremos a GitHub, accederemos a nuestra cuenta y en la esquina superior derecha abra un icono + donde al darle click, nos aparecera la opción de crear un nuevo repositorio. Tambien sueles encontrar un boton Verde que tambien tiene la misma funcionalidad.

Si no menciono algo aquí, no le muevas.

2. Nos llevara a una página nueva para los detalles de nuestro repo. Agregaremos un nombre. En este caso podriamos poner `Primer-Repo`.

3. Dejalo en Public.

4. Te pregunta si quieres inicializar el repo con un archivo README, nuestra carpeta ya tiene ese archivo así que no seleccionaremos la casilla.

5. El .gitignore son carpetas/archivos que no quieres que se suban al repositorio de GitHub. Más adelante aprenderas de ellos.

6. Licencia en None

7. Daremos click al boton verde [Create Repository]

Una vez creado tu respositorio, te pondran las instrucciones para enlazar tu repo de GitHub con el de tu computadora.

Seguiremos el tutorial de la sección **…or create a new repository on the command line** donde vemos que algunos pasos ya los realizamos. 

Nos indica que debemos definir una rama Main con el comando: 

```git
git branch -M main
```

Para entender un poquito las Ramas veremos la siguiente imagen:

<img src='./assets/Branchs.png'>

En los equipos de desarrollo, y dependera mucho de su manejo, utilizaran ramas para poder trabajar sus cambios.

Esta es como la base donde podemos ver que tenemos 4 ramas: Main, Release, Develop y Features.

* Main: La rama main es la rama principal (antes llamada Master) y suele utilizarse como la rama de producción. Esto se refiere a que seran los cambios que estaran ya desplegados en nuestra aplicación.

* Release: Suele no estar presente pero depende de tu equipo y es para la preparación a la hora de unir algún cambio proveniente de la rama de develop para que este listo para incorporarse a prod.

* Develop: Rama utilizada para los cambios de los desarrolladores, bugs que hayan salido.

* Features: Esta como otras ramas de apoyo, te ayudan con caracteristicas nuevas, pero depende mucho de la estructura.

Para entender más sobre estas ramas, puedes buscar en internet documentación de todo el Git Flow.

Las ramas empiezan ya a trabajarse cuando participas en un equipo de desarrollo. Mientras estaremos utilizando la rama Main.

Asi que en nuestra terminal si utilizaremos el comando:

```git
git branch -M main
```

Despues nos dice que utilizemos git remote que nos ayudara a realizar la sincronización del repo de Github con nuestra carpeta con nuestro repo local. Utilizaremos el comando que nos aparece ahí ya que ese incluye nuestro nombre se usuario y el nombre del repo. 

```git
git remote add origin https://github.com/TUNOMBRE/Primer-Repo.git
```

Si todo salio bien, no nos regresara nada.

Ya tenemos enlazado nuestra carpeta local con nuestro repo de GitHub, pero nos faltan subir esos cambios que hicimos en nuestro repo local.

Para eso nos indica que usemos el comando. 

```git
git push -u origin main
```

Este comando subira los commits realizados a nuestro repo de GitHub en la rama Main. 

Para esto nos pedira autentificarnos si no, todos podrian subir carpetas a repos de cualquier persona.

Nos dice que abrira una ventana en el navegador predeterminado para hacer la autentificación.

<img src='./assets/GitHub.png'>

Despues de poner nuestro usuario, nos aparecera lo siguiente:

<img src='./assets/Autentificacion.png'>

Y en nuestra consola aparecera que se realizaron los cambios perfectamente.

Ya podemos ir a nuestra página del repo donde aparecian las instrucciones y refrescar la página y ver nuestro primer archivo ¡Ya subido!.

<img src='./assets/Primer_Repo.png'>


## ¡¡Felicidades!!

<img src='https://i.gifer.com/3LT1.gif'>

