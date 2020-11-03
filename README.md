# Vehiculo-Guia-Autonomo-Experimental
Este proyecto está orientado a la creación de un vehiculo que pueda desplazarse por las instalaciones de un edificio guiando a las personas en su recorrido.
Los materiales utilizados en este proyecto son:

Placa Jetson Nano

Tarjeta Micro SD 64GB

Adaptador USB para memoria micro SD

Estructura metálica para montar un vehículo robótico

Tarjeta de expansión 

Cámara IMX219-160

Placa Wi Fi

Motorreductores

Neumáticos 4 piezas

Servos

Nudillo de dirección 2PCS

Rodamiento 4PCS

Rótula de plástico 4PCS

Barra de tracción M3 2PCS

Cargador de batería de 12,6 V 

Ventilador de enfriamiento 4010

Lector de tarjetas micro SD

Tornillos

# Armado del prototipo
(En las figuras se ven elementos destacados del robot)

En la siguiente figura se ve la computadora con sus conectores:

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/placa%20Jetson%20Nano%20github.jpg)

En la siguiente figura se ve la cámara utilizada en el proyecto:

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/camara%20github.jpg)

En la siguiente figura se ve la cámara memoria MSD utilizada en el proyecto la que debe tener 16 GB o de mayor capacidad:

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/conecci%C3%B3n%20MSD%20github.jpg)

En la siguiente figura se ve la placa Wifi utilizada en el proyecto la que nos permitirà conectar en red con la PC , notebook o celular:

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/WI%20FI%20jetson%20nano%20github.jpg)

En la siguiente figura se ve los actuadores utilizados en el proyecto:

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/actuadores%202020%20github.jpg)

En la siguiente figura se ve las conexiones utilizadas para configurar la computadora:

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/conecciones%20github.jpg)

En la siguiente figura se ve el shield para conectar los motores y el servo del robot:

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/motor%20shield%20github.jpg)

# Grabado del software en la tarjeta micro SD

En primera instancia formateamos la memoria con SD Formater mediante el adaptador de memoria enchufado a un puerto USB de la PC:

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/Configuraci%C3%B3n%20de%20la%20MSD%202%20github.jpg)

Luego utilizamos USB Image Tool para grabar la imagen del sistema que utilizará el robot mediante el adaptador USB de memoria enchufado a un puerto USB de la PC :

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/USB%20Image%20Tool%20github.jpg)

# Armado de la máquina virtual con Ubuntu 18.04 y Jupiter para  trabajar con el código que utilizará el robot.

Cabe destacar que tanto Jetson Nano como Blackberry utilizan el sistema operativo Linux por lo que es necesario contar con una máquina que utilice este SO.  Si bien hay diversas manera de obtener una máquina vbrtual entre las que podemos citar la utilización de software específico para realizar la virtualización como VMware, VirtualBox y otros, tambien se podría utilizar dual boot en la PC para seleccionar un arranque con Linux, en este caso uitlizaremos la posibilidad que nos brinda Windows 10 de ejecutar una terminal de Ubuntu como una aplicación.

Inicialmente debemos ener actualizado Windos 10 e instalar el Subsistema de Windows para Linux con:

dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

Luego debemos habilitar la característica opcional Plataforma de máquina virtual en Windos ejecutando en el power Shell el comando:

dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

para luego descargar el paquete de Linux, Ubuntu 18.04 LTS

Tendeemos de ese modo Ubuntu 18.04 en el escritorio de windows con un acceso que se verá de la siguiente manera

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/icono%20ubuntu.jpg)




























