# Plantilla para proyectos con Flutter.

Esta es una plantilla vacía creada en la clase de Aplicaciones Móviles, la cual nos servirá para futuros proyectos 
dentro de la clase.

# ¿Cómo subir proyectos a Git? Tutorial en Español.

Lo primero que debes hacer, es abrir tu editor de código favorito, la opción más
utilizada es Visual Studio Code. Posteriormente abres tu proyecto que deseas subir a git.

Abrimos una terminal. Puedes abrir la terminal por defecto que tienen todos los Sistemas Operativos en 
cualquier plataforma. En mi caso, uso la de VS Code, que ya viene integrada.

Sigue los siguientes pasos:

**Paso 1.** Con el siguiente comando `git init` inicializamos proyecto en un repositorio local, ya que sin 
este comando, por obviedad no podremos subir ese proyecto a git.

**Paso 2.** El siguiente paso es hacer `git add` para indicarle a git que queremos subir todos los archivos.

> [!IMPORTANT]
> Después de la palabra del comando `git add` se le tiene que indicar alguno de estos argumentos:
> 
> a) `git add .`(espacio y punto) indica a Git que se requiere cargar absolutamente todos los archivos de tu proyecto.
> 
> b) `git add <nombre_archivo>` indica a Git que solamente se desea subir ese archivo en cuestión.

**Paso 3.** Puedes hacer un `git status` para ver los archivos que se van a modificar o cargar, y también para ver la
rama en la que te encuentras.

**Paso 4.** Luego, hacemos un commit con el siguiente comando `git commit`, esto es para confirmar los cambios que se van
a realizar.

> [!IMPORTANT]
> Después de la palabra del comando `git commit` se le tiene que indicar este parámetro:
> 
> `git commit -m "mensaje personalizado"`. El parámetro `-m` nos sirve para indicar un mensaje entre comillas y puede ser
> una guía para el usuario. Por ejemplo indicar una versión del proyecto, o indicar algún mensaje que represente el contenido
> de la versión de archivos a subir, etc.

**Paso 5.** Después de hacer un commit, se tiene que verificar la rama en la que te encuentras haciendo uso del comando
`git branch`. Este comando te mostrará todas las ramas activas en ese repositorio, y la rama en la que el usuario está
ubicado se distingue por el aterisco y por el color de dicha rama.

**Paso 6.** Si deseas cambiar de rama, puedes hacerlo mediante el comando `git checkout nombre_rama`, este te va a 'direccionar' a la rama que desees en caso de que tengas más de una rama.

**Paso 7.** Ya que estés seguro de la rama en la que se subirá tu proyecto, con el siguiente comando `git remote add origin <url.git>`.

### Ejemplo del comando del paso 7.

El comando como ejemplo quedaría de la siguiente manera `git remote add origin https://github.com/NombreUsuario/repositorio.git`

**Paso 8.** Luego, existe el comando `git pull`, que nos permite preparar los archivos para subirlos a git.

**Paso 9.** Por último, hacemos `git push -u origin nombre_rama` para enviar los archivos cargados al repositorio de GitHub.

## Clonar un repositorio

Para clonar un repositorio de Git, es tan sencillo como ir a algún repositorio de www.github.com, copiar el link que aparece en 
la pestaña de Code `(similar a: https://github.com/NombreUsuario/repositorio.git)`, y en la consola hacer un `git clone <url.git>`, posteriormente se van a descargar todos los archivos que tiene el repositorio y los va a guardar en la carpeta ya nombrada dentro de tu computadora.

## SOLUCIÓN A ERRORES

> **No puedo subir otro repositorio a Git ya que la consola me manda un mensaje de error. ¿Cómo le puedo hacer?**
> 
> Con el comando `git remote -v` te van a aparecer algún repositorio con su URL. Es por ello que te marca error,
> para solucionarlo, puedes probar el siguiente comando `git remote remove origin` para eliminar la dirección URL del repositorio
> anterior.
>
> Una vez hecho lo anterior, se puede comprobar de nuevo el comando `git remote add origin [url].git` y si ya no te marca ningún error, > es porque ya se ha eliminado la URL del otro repositorio y posteriormente puedes hacer `git pull` y por último `git push`

# Anexos.

Si ya tienes conocimientos de Git, aquí tienes los comandos rápidos:
```
git init
git status
git commit -m ""
git branch
git checkout
git remote add origin 
git pull
git push -u origin main
git clone 
```

# Referencias ...

Comming Soon ...








