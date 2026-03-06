
Las imágenes están formadas por capas (que son fases en las que se constuyen)

Las imágenes tienen *tags*, es decir etiquetas que nos dice la versión, si no se especifica, se da por entendido que quieres bajar la última versión (latest).


El comando para descargar una imagen es el siguiente:

````
docker pull <image>:<tag>
````

Para buscar una imagen

````
docker search <imagen>
````


Listar imágenes

````
docker images
````

Para saber como se formó una imagen podemos utilizar el comando *history*

````
docker history <image>
````

Para hacer un borrado de imagen *no pueden estar asociadas a contenedores en exec*

````
docker rmi <imagen>

	-f : Fuerzas la eliminación, puedes dejar contenedores sin funcionar
````

Para borrar todas las imágenes que no tienen contenedores asociados:

````
docker image prune 
	-a : Borra todas
	
````

Para crear una imagen a partir de un contenedor es necesario hacer un commit a partir del contenedor de origen

````
docker commit <contenedor> <nombre imagen>
	-a: autor
	-m: mensaje
	 
````

Aveces es normal aplicarle un tag a una imagen, por ejemplo latest a una versióm

````
docker image tag <imagen:tag> <imagen:segundoTag>
````

Para hacer una copia de seguridad de una imagen se puede usar el comando *docker save*

````
docker save  nombre_imagen:tag
	-o nombre_archivo.tar
````

Subir una imagen a un repositorio.
Necesitas etiquetar tu imagen local con tu nombre de usuario para que el repositorio sepa a dónde enviarla.


````
docker tag <imagen> <usuario en repositorio>/ubuntu-apache:v1
````

