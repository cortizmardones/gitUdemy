	Comandos GIT

(Saber la versión de Git)
git --version

(Ayuda en git)
git -help
git help commit (Ayuda con comandos especificos)

(Configuración globales)
git config --global user.name "Carlos Ortiz" (Agrega nombre de usuario)
git config --global user.email "cortizmardones@gmail.com" (Agrega correo a git)

git config --global -e (Ver la información anterior - Me abre un fichero VI <3)
git config --global -l (Aparece la info sin opcion de editar)

(Inicializar GIT - se genera una carpeta invisible)
git init

(En rojo me aparecen los archivos que no he agregado o modificado y estan a la espera de git add)
(En verde me aparecen todos los archivos que agregue con git add . y estan a la espera de commit)
(En plomo todo lo que me falta subir al server con push)
git status
git status -s (Modo silencioso - trae letritas)
git status -s -b (Muestra la rama en la que estoy)

(Agregar archivos al stagin area)
git add .
git add *.png (Agregar solo extensiones especificas)
git add carpeta/ (Agregar archivos dentro de carpetas/folders)

(Elimina archivos del staging area)
git reset nombreArchivo 
git reset *.png (Elimina solo las extensiones especificas)
git reset . (Elimina todo)

(Se crea el snapshot del código)
git commit -m "Comentario"

(Me lleva al último commit) SALVAVIDA
git checkout -- .
git checkout -- ARCHIVO.PNG (Restaura solo un archivo)

(Es para ver el historial de COMMIT que he realizado)
git log
git log --oneline
git log --oneline --decorate --all --graph

(Crear Alias)
git config --global alias.lg "log --oneline --decorate --all --graph"
git lg (Llamando al Alias , va a ejecutar todas las propiedades anteriores que estan delimitadas en "" en el comando anterior)

git config --global alias.s "status -s -b"
git s


(Ver los cambios que hice cuando vuelvo de almorzar y no se que modifique y no he hecho commit)
git diff
git diff --staged


git commit --amend -m "PARA CAMBIAR EL COMENTARIO DEL ULTIMO COMMIT SI ME EQUIVOQUE"

(Para agregar al stage y commitear a la vez)
git commit -am "mensaje"

(Volver en el tiempo)
git reset --soft 860c6c2 (conserva archivos - solo tendria que agregarlos de nuevo al staging y commitear) 
git reset --hard 860c6c2 (Destruye los archivos- ojo con este)
git reset --mixed 860c6c2 (Investigar que hace esta forma)














































	CURSO NORMALIZADO (AYUDA MEMORIA)
git init
git add .
git commit -m "snapshot01"
git remote add origin https://github.com/BlaBlaBla
git push -u origin master

	SOLUCIÓN CRLF
git config core.autocrlf true










