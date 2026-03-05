
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
