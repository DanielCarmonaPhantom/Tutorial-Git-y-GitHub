<img src='./assets/Titular.png'>

Contenido:
1. Terminal
2. Descarga
3. Configuración
4. Introducción a Git

## 1. Terminal
Antes de instalar, visualizaremos si ya tenemos instalado git, ya que en algunos sistemas operativos ya lo incorpora.

Podemos verificar si ya lo tenemos instalado utilizando una terminal de comandos. La terminal nos ayuda a ejecutar comandos tipo peliculas de hollywood que para nada es difícil y a lo largo de tu vida como dev, iras aprendiendo a manejar.

**Windows**: La terminal que trae por defecto es cmd, tambien puedes utilizar otras terminales que podras descargar más adelante. 

Para abrir cmd puedes darle al buscador de windows y buscar cmd. Si te encuentras en un windows que no tiene buscador, puedes utilizar la tecla `[Windows + R]` y se abrira una ventana donde deveras escribir `cmd` y automaticamente se te abrira la terminal de windows.

**Mac**: En la lupa superior de busqueda, podemos buscar `terminal` y seleccionar la aplicación.

**Linux**: Dependiendo de cada distribución, pero en un plano general, la podemos encontrar en nuestras herramientas como `Terminal`.

---

Una vez dentro de nuestra terminal, utilizaremos el comando:
```Bash
git --version
```

Este comando nos ayudara a visualizar la versión de git que en su caso, tuvieramos instalada.

Puede que no tengas git instalado, así que seguiremos con el tutorial.

## 2. Instalación

### Instalación de Windows y Mac

Iremos al [sitio oficial de git](https://git-scm.com/downloads) y automaticamente nos selecciona el sistema operativo, daremos click en Descargar.

Cuando vayamos a instalar, nos ira pregutando cual sera la configuracíon. Puedes dar next a todo sin problema.

### Instalación en Linux

Nos iremos a la terminal y actualizaremos la lista de paquetes con el comando:
```Bash
sudo apt-get update
```
y despues
```Bash
sudo apt-get upgrade
```
Una vez teniendo actualizado nuestros paquetes, actualizaremos el git de nuestra maquina con:
```Bash
sudo apt-get install git
```

### Verificar Git
Verificaremos si ya tenemos instalado git con el comando que usamos más arriba:
```Bash
git --version
```
y nos aparecera ya la version de git instalada.
```prompt
2.36.0
```

## Configuración

Para definir el usuario y correo que estaremos utilizando y probablemnte el que se una con GitHub, tendremos que configurar nuestro entorno modificando las variables de nombre y correo de git.

Para esto, dentro de nuestra terminal utilizaremos el comando y modificando lo que esta dentro de las `""`: 
```Bash
git config --global user.name "Aqui va tu nombre. Mucho Ojo"
```
y para configurar tu correo, recomendable que sea el que ya tengas en tu cuenta de Github:
```Bash
$ git config --global user.email "Aqui va tu correo"
```

## Introdución a Git

Git nos ayudara a manejar las versiones de estados sobre nuestros archivos. ¿A que se refiere estados?. ¿Recuerdas lo que dicen de TesisFinal y luego es TesisFinal2 y despues es TesisFinalFinal? lo que te ayuda git es a trabajar esas versiones que vas manejando. Ahora imaginate que ese archivo no solo lo editas tu, si no más personas, entonces para poder ver los cambios que se realizen, git te permite visualizar lo que ha subido cada quien. Tambien puedes saltar en el tiempo, volviendo a un estado anterior y empezando desde ahí. 

### Creando un repositorio

Un repositorio sera una carpeta donde se trabajara todo este control de versiones. 
Para inicializar un repo, primero debemos situarnos en la carpeta que desemos tener este control de versiones.

#### 1. Crearemos una carpeta en el escritorio se llame: `Primer-Repo`. 

La carpeta `Primer-Repo` la estaremos definiendo para utilizarlo con GitHub.

Regularmente se crean estos repos en el escritorio, pero esto ya depende de donde te guste trabajar tus carpetas.

#### 2. Debemos situarnos en la carpeta.

Para "situarnos" debemos movernos dentro de la consola.

Cuando inicias la terminal, esta te situa en un punto especifico de tu computadora. Regularmente en la carpeta del Usuario. 


En Windows nos sale la ruta donde estamos posicionados:

```Bash
C:\User\Daniel>
```

Pero en otros sistemas solo nos aparece el nombre y computadora
```Bash
Daniel@Mycomputadora ~ %
```

Para visualizar en donde te encuentras puedes utilizar el siguiente comando.

Para Mac y Linux:
```Bash
pwd
```

El resultado sera la carpeta en donde la terminal esta situada. 

Puedes visualizar los archivos que contiene la carpeta en donde te cuentras , utilizando:

Para Windows: 
```Bash
dir
```

Para Mac y Linux:
```Bash
ls
```

Ahora que sabes que archivos contiene la carpeta en donde estamos, nos vamos a mover a la carpeta `Desktop` donde se encuentra la carpeta `Primer-Repo`.

Para podernos mover entre carpetas utilizaremos el comando `cd` + espacio + "Nombre de la carpeta" a la que nos vamos a mover.

```Bash
cd Desktop
```

Veremos que en nuestro nombre de la terminal nos añadira la carpeta que nos movimos. 

Haremos lo mismo para entrar a nuestro `Primer-Repo`:

```Bash
cd Primer-Repo
```

#### 3. Inicializar el primer respositorio.

Ya una vez que nuestra consola este situada en la carpeta que estaremos trabajando, utilizaremos el comando de git:

```Bash
git init
```

Nota: Recuerda verificar que estas en la carpeta `Primer-Repo` con `pwd` por que aveces uno puede estar en Desktop y dar el `git init` y liarla.  

#### 4. Subiendo nuestro primer archivo.

Una vez inicido el git, ya podremos utilizar el manejo de versiones con nuestros archivos.

Aqui ya estaremos utilizando nuestro editor de código. 

Para este ejemplo utilizaremos VS CODE pero recuerda que es el de tu preferencia.

Los pasos son muy similares a otros editores.

Abriremos VS CODE y nos iremos a File y ahí seleccionaremos `Open Folder` y buscaras nuestro repo, lo seleccionas y le das a boton [Seleccionar carpeta] o [Abrir]. Si le das enter, solo entraras a la carpeta como si fueras a buscar adentro. 

. Tambien en tu terminal puedes teclear:
```Bash
Code 
```
y se abrira una ventana de VS CODE ya en la carpeta `Primer-Repo`. Aveces no esta configurado esta opción pero es muy facil de hacerlo.

Ya dentro de nuestro VS COde de lado izquierdo tenemos un icono llamado `Explorer` donde podremos visualizar todas las carpetas y archivos que estan dentro de la carpeta `Primer-Repo`.


