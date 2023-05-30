# comandos útiles de GIT

1- git init 
    Inicializa el repositorio.
    Crea un subdirectorio .git en el directorio de nuestro proyecto con todo lo que necesita GIT para nuestro proyecto. 
    Este directorio es oculto.

2- git add .
    Prepara todos los archivos nuevos o con cambios para una nueva foto (commit) del proyecto en el repositorio.
    En realidad sube todos los archivos modificados o nuevos a un escenario conocido como stage y los deja preparados para un commit.

3- git reset .
    Tira para atrás todo lo preparado por el comando add . 

4- git commit
    Sube la foto preparada en el stage al repositorio.
    Lo normal es indicar un comentario, para eso se escribe:  git commit -m "<comentario>"
        donde <comentario> debe sustituirse por lo que indiquemos en el comentario.
    
5- git checkout -- .
    Recupera todo lo que tenemos en el repositorio de nuestro proyecto machacando lo que tenemos en nuestro proyecto.
    Incluso los archivos borrados se hacen fácilmente recuperables.

6- git log
    Nos permite ver todo el listado de commits que hemos ido haciendo sobre nuestro proyecto.
    Para salir del scroll presentado con los commits tocar la tecla Q

7- git commit --amend
    Presenta en la terminal el comentario del último commit y nos permite modificarlo e insertar nuevas líneas.
    Para entrar en el modo de modificación o inserción de texto pulsar la tecla I
    Para guardar los cambios y salir:
        ESCAPE
        :wq!

            donde: 
                  : -> línea de comandos
                  w -> write
                  q -> quit
                  ! -> ejecutar inmediatamente

8- git checkout -b <rama>            
    Crea una nueva rama (-b de branch) con el nombre: <rama> en la que pone todo nuestro repositorio

9- git branch
    Muestra las ramas que tenemos en el proyecto y nos indica en la que estamos actualmente trabajando

10- git checkout <rama>
    Cambia nuestro proyecto a la rama especificada en <rama>, sea la principal o no.
    Automáticamente los archivos corresponderán a esa rama, desapareciendo los que no lo sean y apareciendo los que no estuvieran en el momento actual.

11- git merge <rama>
    Realiza un commit o merge de los cambios hechos en la rama a la rama master o principal.

12- git branch -d <rama>
    Borra la rama especificada por <rama>

13- git remote add origin <url remota>
    Vincula el repositorio actual al que tenemos en GitHub con la URL de acceso: <url remota>
    ej. git remote add origin https://github.com/vangeyper/vangeyperGit.git

14- git branch -m <NuevoNombre>
    Cambia el nombre de la rama principal a lo indicado en <NuevoNombre>

15- git push -u origin <rama>
    Sube al repositorio externo de GitHub asociado la rama especificada en <rama>
    Con git push también subiría los cambios al repositorio de la rama actual      

16- git commit -am "<comentario>"
    Realiza un git add .   y un git commit -m "<comentario>" al mismo tiempo.

CAMBIAR URL REMOTA EN GIT
GIT es uno de los controles de versiones de código más utilizado en todo el mundo por los desarrolladores y programadores. Es ciertos casos pueden surgir algunos inconvenientes en su uso, por ejemplo se puede tener la necesidad de cambiar la URL remota del repositorio con el cual se está trabajando actualmente.

Para resolver este inconveniente en este breve tutorial te vamos a explicar cómo cambiar la URL remota con GIT, de forma tal que puedas apuntar a otro repositorio. Esto también puede ser muy útil cuando se desea cambiar de usuario a hacer un push.
    
Cómo cambiar la URL remota en GIT utilizando un comando
Como veremos a continuación realizar esta acción es una tarea muy sencilla, solamente vamos a necesitar ejecutar el comando git remote set-url segudo por la nueva URL. En caso de querer indicar un nombre de usuario y una contraseña hay que remplazar el name y el password correspondiente.


git remote set-url origin https://name:password@github.org/repo.git
Para el caso de no querer indicar un usuario y una contraseña simplemente se puede sacar esos datos de la URL, como se muestra a continuación.


git remote set-url origin https://github.org/repo.git
Eso es lo que simplemente hay que hacer a la hora de cambiar la URL de un repositorio remoto, para poder hacer los push correctamente.





    

