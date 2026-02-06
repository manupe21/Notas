
# Contenedor

El contenedor se ejecuta dentro de un SO como un proceso, es parecido a una máquina virtual, solo que en vez de un SO completo solo coge las librerías y dependencias que necesita para su ejecución.

Se ejecuta como un proceso.

Se puede hacer un *commit* del contenedor y guardarlo como imagen.

## Entrypoint

Es el comando que se ejecuta al iniciarse un contenedor. Suele aparecer en la pestaña "Command" dentro de un docker ps

![[{DDD09418-4C4D-4E2A-AA6F-0B21A196BEE3}.png]]



# Imagen

Las imágenes son la librerías y binarios que necesita un contenedor para desplegarse. Suelen estar en repositorios remotos y se tienen que descargar.
Las imágenes se suelen generar con *dockerfile* 

![[Pasted image 20260206104619.png]]

