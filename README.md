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


    

