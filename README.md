# ¿Cómo subir proyectos a Git? Tutorial sencillo explicado en español 2024.

Lo primero que debes hacer, es abrir tu editor de código favorito, en lo personal uso Visual Studio Code.
Posteriormente abres tu proyecto que deseas subir a git.

Abrimos una terminal. Puedes abrir la terminal por defecto que tienen todos los Sistemas Operativos en 
cualquier plataforma. 
En mi caso, uso la de VS Code, que ya viene integrada.

Sigue los siguientes pasos:

Paso 1. Con el siguiente comando `git init` inicializamos proyecto en un repositorio local, ya que sin 
este comando, por obviedad no podremos subir ese proyecto a git.

Paso 2. El siguiente paso es hacer `git add` para indicarle a git que queremos subir todos los archivos.

> [!IMPORTANT]
> Después de la palabra del comando `git add` se le tiene que indicar alguno de estos argumentos:
> 
> a) `git add .`(espacio y punto) indica a Git que se requiere cargar absolutamente todos los archivos de tu proyecto.
> 
> b) `git add <nombre_archivo>` indica a Git que solamente se desea subir ese archivo en cuestión.

Paso 3. Puedes hacer un `git status` para ver los archivos que se van a modificar o cargar, y también para ver la
rama en la que te encuentras.

Paso 4. Luego, hacemos un commit con el siguiente comando `git commit`, esto es para confirmar los cambios que se van
a realizar.

> [!IMPORTANT]
> Después de la palabra del comando `git commit` se le tiene que indicar este parámetro:
> 
> `git commit -m "mensaje personalizado"`. El parámetro `-m` nos puede servir para saber que archivos hemos subido a nuestro git

Paso 5. Después de hacer un commit, se tiene que verificar la rama en la que te encuentras haciendo uso del comando
`git branch`. Este comando te mostrará todas las ramas activas en ese repositorio, y la rama en la que el usuario está
ubicado se distingue por el aterisco y por el color de dicha rama.

    Paso 5.1. Si deseas cambiar de rama, puedes hacerlo mediante el comando `git checkout nombre_rama`, este te va a 'direccionar' a la rama que desees en caso de que tengas más de una rama.

Paso 6. Ya que estés seguro de la rama en la que se subirá tu proyecto, con el siguiente comando `git remote add origin https://github.com/NombreUsuario/repositorio.git`.

### Ejemplo del comando del paso 6.

El comando como ejemplo quedaría de la siguiente manera `git remote add origin https://github.com/NombreUsuario/repositorio.git`

Paso 7. Luego, existe el comando `git pull`, que nos permite preparar los archivos para subirlos a git.
Paso 8. Por último, hacemos `git push -u origin nombre_rama` para enviar los archivos cargados al repositorio de GitHub.

**Solución al momento de subir el proyecto a nuestro repositorio.**

¿Si tengo problemas para subir el repositorio, cómo le hago?

R. Puedes probar el siguiente comando `git remote remove origin` para eliminar la dirección URL del repositorio anterior de Git, ya que este te causa conflicto con el repositorio actual.









