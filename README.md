# Docker

1. Bajar la imagen Docker llamda "hello-world"


> docker pull hello-world

Ejecutar imagen de hello-world:

> docker run hello-world

# Docker & SQL

1. Bajar la imagen Docker de SQL Server
 > docker pull mcr.microsoft.com/mssql/server:2022-latest
 
2. Ejecutar la imagen de SQL Server en un contenedor con el usuario y password de nuestra eleccion
 > docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=Passw0rd" -p 1433:1433 -d mcr.microsoft.com/mssql/server:2022-latest
 
 # GIT
 
 Para subir los cambios de un repositorio local a un repositorio remoto, primeramente, se ejecuta:
 > git init
 
 despues se asocia el repositorio local con el remoto, ejecutando el comando:
 > git remote add "link del repositorio"

 Una vez ligado el repositorio remoto al local para subir cambios o subir archivos, se hace lo siguiente:
	1. Haces un stage de los cambios realizados al repositorio con:
		> git add .
	
	2. Una vez hecho el stage de los cambios, se procede a hacerles commit con:
		> git commit -m "Este es un commit"
	3. Finalmente, se migran los cambios del repositorio local al remoto con:
		> git push origin master