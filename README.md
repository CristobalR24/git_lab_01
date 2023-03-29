Git
Cristobal Rodriguez


#comandos 
git init: inicializa un repositorio

git add [archivo] / git add . : permite subir archivos al staging area*

git commit -m "mensaje del commit": permite "guardar" los cambios realizados

git diff [archivo] / git diff [hash] [archivo]: permite visualizar los cambios realizados entre un commit y otro

git branch [nueva_rama] / git branch [nueva_rama] [commit base]: permite crear una nueva rama

git checkout [branch]: permite movernos entre ramas 

git checkout -b [branch]: permite crear una nueva rama y hacer checkout

git revert: regresar a un punto de la historia y realiza un commit, los cambios luego de este punto siguen 
	    apareciendo como unstaged

git reset: regresar a un punto de la historia y no realiza un commit
	git reset --soft: asume que los cambios siguientes no existen
	git reset --hard: borra de la existencia los cambios siguientes
