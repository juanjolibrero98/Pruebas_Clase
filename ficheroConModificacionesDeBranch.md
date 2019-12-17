#Este fichero es para mostrar el codigo en terminar, donde se muestran los cambios de rama

...:~$ cd Repositorio_Pruebas_Clase/

...:~/Repositorio_Pruebas_Clase$ git clone https://github.com/....
Clonando en 'Pruebas_Clase'...
warning: Pareces haber clonado un repositorio sin contenido.

...:~/Repositorio_Pruebas_Clase$ cd Pruebas_Clase/

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ nano README.md

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ mkdir bin

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ ls
bin  README.md

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git branch rama1
fatal: Nombre de objeto no valido: 'master'.

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git branch

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git branch rama1
fatal: Nombre de objeto no valido: 'master'.

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git branch "rama1"
fatal: Nombre de objeto no valido: 'master'.

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git add .

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git status
En la rama master

No hay commits todavía

Cambios a ser confirmados:
  (usa "git rm --cached <archivo>..." para sacar del área de stage)

	nuevo archivo:  README.md

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git commit -m "Version"
[master (commit-raíz) c19ecd9] Version
 1 file changed, 3 insertions(+)
 create mode 100644 README.md
 
...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git branch "rama1"

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git branch 
* master
  rama1
  
...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git chechout rama1
git: 'chechout'no es un comando de git. Mira 'git --help'.

El comando mas similar es
	checkout
...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git checkout rama1
Cambiado a rama 'rama1'

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ nano README.md 

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ cd bin/

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase/bin$ nano README.md

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase/bin$ cd ..

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git add .

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git commit -m "Archivos actualizados"
[rama1 ccc54dd] Archivos actualizados
 2 files changed, 2 insertions(+), 1 deletion(-)
 create mode 100644 bin/README.md
 
...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ nano README.md 
...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git add .

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git commit -m "Control version"
[rama1 a172622] Control version
 1 file changed, 1 insertion(+), 1 deletion(-)
 
...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git checkout master
Cambiado a rama 'master'
Tu rama esta basada en 'origin/master', pero upstream ha desaparecido.
  (usa "git branch --unset-upstream" para arreglar)
  
...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ nano README.md 

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git merge rama1
Actualizando c19ecd9..a172622
Fast-forward
 README.md     | 2 +-
 bin/README.md | 1 +
 2 files changed, 2 insertions(+), 1 deletion(-)
 create mode 100644 bin/README.md
 
...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ nano README.md 

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git branch
* master
  rama1
  
...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git branch -d rama1
Eliminada la rama rama1 (era a172622)..

...:~/Repositorio_Pruebas_Clase/Pruebas_Clase$ git branch
* master

