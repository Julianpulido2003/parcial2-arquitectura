# parcial2-arquitectura
Parcial Diseño y Arquitectura de software
6
a. Lo primero que hay que hacer es descargar el contenedor de Mysql con el siguiente comando.

$ docker run -d -p 33060:3306 --name root -e MYSQL_ROOT_PASSWORD=clave 
y a la vez hay que hacer la configuracion del archivo yml en donde se configuran el puerto, usuario y contraseña.
9. Dockerfile 
 FROM openjdk:19-oracle

COPY ./build/libs/shop-api-0.0.1-SNAPSHOT.jar /app.jar

EXPOSE 8010

ENTRYPOINT ["java","-jar","/app.jar"]
