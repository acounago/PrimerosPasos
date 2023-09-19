**1. Descarga la imagen 'ubuntu y comprueba que está en tu equipo**

*Comando para la descarga de la imagen de ubuntu:* 
  *#docker run -it --name asir_2 ubuntu:bionic-20230530 bash*
*Comando para la comprobación de que está en nuestro equipo:*
  *#docker images*


**2. Crea un contenedor sin ponerle nombre. ¿está arrancado? Obtén el nombre**

Para crear el contenedor sin nombre:
  *#docker run ubuntu bash*
*No se está arrancando.*
*Comando para obtener el nombre:*
  *#docker ps -a*


**3. Crea un contenedor con el nombre 'ubu1'. ¿Como puedes acceder a él?**

*Comando para crear el contenedor y acceder a el:*
  *#docker run -it --name ubu1 ubuntu bash*
*En el caso de querer acceder a el desde fuera, usamos este comando:*
  *docker exec -it ubu1 bash*


**4. Comprueba que ip tiene y si puedes hacer un ping a google.com**


*Instalamos el paquete #net-tools y con el comando #ifconfig comprobamos que la ip es: 172.17.0.4*
*Instalamos el paquete #iputils-ping y con el comando #ping comprobamos que sí podemos hacer ping a google.com*

**5. Crea un contenedor con el nombre 'ubu2'. ¿Puedes hacer ping entre los contenedores?**

*Instalamos el paquete  #iputils-ping y con el comando #ping comprobamos que si se puede hacer ping entre los dos contenedores.*



**6. Sal del terminal, ¿que ocurrió con el contenedor?**

*El contenedor se detiene*


**7. ¿Cuánta memoria en el disco duro ocupaste? ¿Hay alguna herramienta de docker para calcularlo?**

*Ocupamos 226.6MB*
*El comando es: docker system df*

**8. ¿Cuanta RAM ocupan los contenedores? Crea cuántos contenedores necesites para calcularlo.**

*Usamos el comando #docker stats para comprobarlo y vemos que ocupan:49 MiB*



