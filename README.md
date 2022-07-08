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