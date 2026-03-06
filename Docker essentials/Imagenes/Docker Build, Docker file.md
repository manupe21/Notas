
# Docker file

Son una serie de instrucciones que describen como crear una imagen

* Instrucciones más importantes
	* FROM: Imagen base sobre la que se va a construir
	* RUN: Ejecuta comandos en la imagen
	* COPY: Copia archivos del host a la imagen
	* WORKDIR:  Directorio para el resto de instrucciones
	* CMD: Comando a ejecutar al instanciar la imagen
	* ENTRYPOINT: Lo mismo que CMD pero no se puede sobreescribir

## Ejemplo de archivo dockerfile 

Instrucciones para el fichero: 
- Base: alpine.
- Directorio de trabajo: /app.
- Puerto expuesto: 8080.
- Comando por defecto: top

````sh
vim Dockerfile
------------------------------
FROM alpine:latest
WORKDIR /app
EXPOSE  8080
ENTRYPOINT ["top"]

````
