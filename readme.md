comandos

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto
$ mkdir Practica2

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto
$ cd  Practica2

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2
$ git config --global user.name FreddyUnemi2025

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2
$ git config --global user.email fbravor2@unemi.edu.ec

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2
$ git config --global --list
user.email=fbravor2@unemi.edu.ec
user.name=FreddyUnemi2025
credential.helper=manager
push.autosetupremote=true


Ahora se elimina la cuenta de git del windows con el administrador de credenciales o Credential Manager.
Buscas el que dice https://github.com y lo eliminas ahora podras subir en una nueva cuenta


# Crear, subir y sincronizar el repositorio

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2
$ git init 
Initialized empty Git repository in C:/Users/Freddy/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2/.git/

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git add .

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git commit -m "Readme agregado"
[master (root-commit) e77f38b] Readme agregado
 1 file changed, 20 insertions(+)
 create mode 100644 readme.md

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>


Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git remote add PracticaDeTaller https://github.com/FreddyUnemi2025/PracticaDeTaller

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git push PracticaDeTaller
remote: Permission to FreddyUnemi2025/PracticaDeTaller.git denied to FredBrave.
fatal: unable to access 'https://github.com/FreddyUnemi2025/PracticaDeTaller/': The requested URL returned error: 403

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git push PracticaDeTaller
info: please complete authentication in your browser...
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 456 bytes | 456.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/FreddyUnemi2025/PracticaDeTaller/pull/new/master
remote:
To https://github.com/FreddyUnemi2025/PracticaDeTaller
 * [new branch]      master -> master
branch 'master' set up to track 'PracticaDeTaller/master'.

# Descargar nuevos cambios
Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (rama-para-invitados)
$ git fetch
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 5 (delta 0), reused 5 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (5/5), 706 bytes | 50.00 KiB/s, done.
From https://github.com/FreddyUnemi2025/PracticaDeTaller
   695926e..3595308  rama-para-invitados -> PracticaDeTaller/rama-para-invitados      

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (rama-para-invitados)
$ git pull
Updating 695926e..3595308
Fast-forward
 index.html | 13 +++++++++++++
 1 file changed, 13 insertions(+)
 create mode 100644 index.html

