#Git

autor: Cristobal Rodriguez

#Conceptos

control de versiones: permite mantener un historial de cambios en los archivos evitando la perdida de datos.

git: herramienta que nos permite realizar el control de versiones.

ramas: fragmentos o ramificaciones de la aplicacion, permiten  organizar el trabajo en diferentes funcionalidades.

merge: proceso de combinar dos o más ramas en una sola.
	
	#merge 
	merge automatico: se da cuanto git no encuentra ningun conflicto entre las ramas y procede a unirlas sin 
			  ningun inconveniente.
	merge manual: en el caso de que hayan conflictos, git pedira al usuario que corrija los cambios manualmente
		      antes de realizar el merge.

repositorio remoto: sitio donde se centraliza el trabajo que es accesible para quienes esten autorizados, puede 
		    ser publico o privado.

pull request: solicitud para subir cambios al repositorio y hacer merge.

staging area: donde se ubican localmente los cambios a realizar, esta en la carpeta.

#Comandos 

git init: inicializa un repositorio.

git add [archivo] / git add . : permite subir archivos al staging area*.

git commit -m "mensaje del commit": permite "guardar" los cambios realizados.

git diff [archivo] / git diff [hash] [archivo]: permite visualizar los cambios realizados entre un commit y otro.

git branch [nueva_rama] / git branch [nueva_rama] [commit base]: permite crear una nueva rama.

git checkout [branch]: permite movernos entre ramas. 

git checkout -b [branch]: permite crear una nueva rama y hacer checkout.

git revert: regresar a un punto de la historia y realiza un commit, los cambios luego de este punto siguen 
	    apareciendo como unstaged.

git reset: regresar a un punto de la historia y no realiza un commit.
	   git reset --soft: asume que los cambios siguientes no existen.
	   git reset --hard: borra de la existencia los cambios siguientes.

git remote add [nombre repositorio] [direccion url del repositorio remoto]: añade un repositorio remoto.

git merge [rama a unir]: permite incorporar los cambios a su origen.
