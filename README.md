# DNS-Docker-compose

## Configura un contenedor coa imaxe oficial de bind9 usando docker-compose.

Lo primero que se hara es en la terminal utilizar el comando `gedit docker-compose.yaml ` Se nos abrira el editor de texto y se procede a desarrollar el `.yaml` para crear el contenedor con la imagen bind9.

-Services:Se utilizara varios parametros comenzamos comenzando que se le dara un nombre, luego la *image* la cual se definira la que se pide en esta practica, *container_name* donde se le dara nombre al contenedor como su nombre lo indica, *ports* utilizaremos los puertos tcp y udp lo cual se le indica 54:54 en este caso porque se esta trabajando en maquina virtual sino 53:53 para que las consultas DNS se puedan realizar, *networks* se repite el nombre de la red.
-restart: `always` asegura que el contenedor se reinicie automáticamente si se detiene inesperadamente.

-Networks: definimos la red que en mi caso la llame `bind9` que utilizara el controlador, luego el `driver` lo defini como *briged* para que cree un entorno de red privada, para que el contenedor pueda comunicarse con otros contenedores en la misma red. 