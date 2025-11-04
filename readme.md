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

# Actualizar con commits y subir

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git add .

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git commit -m "Readme actualizado #2"
[master b1dde03] Readme actualizado #2
 1 file changed, 60 insertions(+)

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 1.22 KiB | 1.22 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/FreddyUnemi2025/PracticaDeTaller
   e77f38b..b1dde03  master -> master

# Crear Rama

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git checkout -b "Rama para invitados"
fatal: 'Rama para invitados' is not a valid branch name
hint: See `man git check-ref-format`
hint: Disable this message with "git config set advice.refSyntax false"

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (master)
$ git checkout -b "rama-para-invitados"
Switched to a new branch 'rama-para-invitados'

Freddy@DESKTOP-STRSKJA MINGW64 ~/Desktop/Backend Proyects/CONTPRECNGSTS/practicaproyecto/Practica2 (rama-para-invitados)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'PracticaDeTaller/master'.
