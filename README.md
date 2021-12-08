# Proyecto_Blockchain

El primer paso para crear una blockchain propia utilizando python es descargar Anaconda de la página oficial: https://anaconda.org/ , haciendo click en "Download Anaconda" y "Download", en este caso será la versión más actual de 64-bit para Windows.
![image](https://user-images.githubusercontent.com/70983585/145254001-f4a502df-d58c-41a8-8c1c-c8c8d3e6b7db.png)

Durante la instalación de Anaconda le damos siguiente a todo sin olvidar darle "check" en la casilla del path, esto es fundamental para utilizar los "enviroment" más adelante.
![image](https://user-images.githubusercontent.com/70983585/145255560-12c2506a-5d76-4466-a25b-b6eb13857b42.png)

Una vez terminada la instalación, abrimos Anaconda Navigator para crear un nuevo "enviroment" para crear nuestro blockchain, hacemos click en "create", le damos nombre al entorno y seleccionamos la versión de python a utilizar, en este caso ya tenemos creado nuestro "enviroment Blockchain" con python 3.6.13, una vez seleccionado lo anterior, hacemos click en "create" y esperamos a que termine, luego abrimos la consola para utilizar el comando "activate Blockchain" para poder utilizar nuestro entorno.
![image](https://user-images.githubusercontent.com/70983585/145255707-579b2a80-eb54-4087-8c74-25544c1d5ed8.png)

Volvemos a Home y buscamos en la lista el entorno de desarrollo llamado Spyder, el cual utilizaremos para escribir el código del blockchain, hacemos click en "install" y esperamos a que termine.
![image](https://user-images.githubusercontent.com/70983585/145256176-a68b2c8c-eb8d-44be-9aa1-3a3c37c7548b.png)

Como último preparativo, necesitamos instalar la API de Postman desde el sitio oficial de descarga: https://www.postman.com/downloads/ , esta la usaremos para comprobar que las creación y transaciones de los nodos de la blockchain es exitosa.
![image](https://user-images.githubusercontent.com/70983585/145256691-c0cf2f31-809e-46a4-81fd-088cdb0d2c0e.png)

Ya con todo lo anterior podemos utilizar los srcipts de python llamados: amlopesos_5001, amlopesos_5002 y amlopesos_5003 los cuales simbolizan nodos de nuestra blockchain, cada uno con la capacidad de conectarse a los demás, apuntar hacia el nodo anterior guardar o añadir una chain a la cadena, encriptarla, etc. Una vez abiertos en Spyder los ejecutamos seleccionando todo el código y con el shortcut "ctrl + enter", abriendo una terminal de spyder por nodo, probablemente aparezca un mensaje para dar permiso al cual daremos acceso y todo esto con postman abierto.
![image](https://user-images.githubusercontent.com/70983585/145259271-994d0868-5074-4275-8371-2992ee51774a.png)

Como último paso podemos enlazar nuestra blockchain desde postman, en programas más complejos hay scripts en el backend que se encargan de esto y la encriptación de cada chain es mucho más compleja. 
En postman abrimos tres pestañas una para cada nodo que representa una persona o equipo de la red desantralizada, escribimos el url de cada nodo: http://192.168.100.166:5001/ , http://192.168.100.166:5002/ y http://192.168.100.166:5003/ . Añadiendo "get_chain" obtenemos una chain del nodo y comprobamos que esta funcionando.
![image](https://user-images.githubusercontent.com/70983585/145260693-7e2237b4-3fd2-4068-bb9f-58ebbc16cf33.png)

Para descetralizar nuestra red cambiamos de GET a POST usando Body y raw para enviar el nodes.json el cual contiene las direcciones de todos los nodos de nuestra red de la siguiente forma:
![image](https://user-images.githubusercontent.com/70983585/145261029-df384853-82ac-4cde-a0e7-568e9b03b6c0.png)


Con mine_block, podemos minar un bloque desde el nodo donde estemos, con get_chain podemos visualizar la blockchain que hemos creado.
![image](https://user-images.githubusercontent.com/70983585/145261845-9655b2a1-75d0-4e45-86e1-34e24bbc1a14.png)

