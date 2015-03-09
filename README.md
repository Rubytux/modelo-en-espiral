# modelo-en-espiral
Exposición del Modelo en Espiral.

Git es un controlador de versiones, algo que veremos más adelante en la técnica y que nos ayudará a mantener funcional nuestro código en caso de que realicemos cambios que generen errores.

Para gestionar las versiones, no necesitamos "subirlo" a un repositorio en línea como lo es en este caso Github.com, podemos almacenar las versiones de nuestro software de manera local.

## Instalando Git en distros Linux (Kubuntu 14.04)

En la terminal ingresamos e iniciamos el gestionador de versiones:

```
$ sudo apt-get install git
[sudo] password for hernan:(acá ingresamos la contraseña del super usuario).
$ git init
```

Luego configuramos de manera local nuestra cuenta de Git, para registrar los cambios que le hagamos al software.

```
$ git config --global user.name Nombre1 Apellido1
$ git config --global user.email ejemplo@correo.com
```

Luego creamos nuestro los cambios con cada "commit" del código.

```
$ git add . 
$ git commit -m "Primera version"
```

Donde -m indica un mensaje para informar de los cambios hechos entre versiones.

## Revirtiendo un cambios

Sí un commit generó problemas en el funcionamiento del código, podemos revertir todos los cambios hechos en el así:

```
$git log --pretty=oneline
```

Escogemos el hash del commit a revertir y luego digitamos:

```
$git revert codigohashimpresoanteriormente
```


## Descarga del repositorio Git

Para clonar el repositorio, se puede ir a este enlace:

https://github.com/Rubytux/modelo-en-espiral/archive/master.zip

Se descomprime, ejecuta el archivo Index.html que lleva al navegador y yap :)