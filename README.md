# Vehiculo-Guia-Autonomo-Experimental
Autor: Norberto Aramayo

Tutor: [Guzmán Álvarez, César A.](https://scholar.google.com/citations?user=pwRGe0wAAAAJ&hl=es)

# Índice

### 1) [Introducción](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#1-introducci%C3%B3n)
### 2) [Materiales utilizados](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#2-los-materiales-utilizados-en-este-proyecto-son)
### 3) [Armado del prototipo](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#3-armado-del-prototipo-1)
### 4) [Software utilizado](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#4-software-utilizado-1)
#### 4-1 [Software en la tarjeta Micro SD](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#4-1-grabado-del-software-en-la-tarjeta-micro-sd)
#### 4-2 [Armado de la máquina virtual con Ubuntu 18.04 y Jupiter](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#4-2-armado-de-la-m%C3%A1quina-virtual-con-ubuntu-1804-y-jupiter-para--trabajar-con-el-c%C3%B3digo-que-utilizar%C3%A1-el-robot)
#### 4-3 [Instaalción de Jupiter en Ubuntu](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#4-3-instaalci%C3%B3n-de-jupiter-en-ubuntu-1804)
### 5) [Código del vehículo](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#5-inicio-del-trabajo-con-el-c%C3%B3digo-del-veh%C3%ADculo)
#### 5-1 [Repositorio de datos](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#5-1-repositorio-de-datos-1)
#### 5-2 [Tensorflow - Keras](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#5-2-tensorflow---keras-1)
#### 5-3 [Crear carpeta de datos](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#5-3-crear-carpeta-de-datos-1)
#### 5-4 [Administrar carpeta de dato](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#5-4-administrar-carpeta-de-datos)
### 6) [Conducir y entrenar el modelo](https://github.com/NorbertoAramayo/Vehiculo-Guia-Autonomo-Experimental/blob/main/README.md#6-conducir-y-entrenar-el-modelo-1)

## 1) Introducción

Este trabajo está orientado a crear un vehículo guía autónomo experimental que sirva para recorrer y guiar a los vasitantes de empresas o instituciones por las diferentes instalaciones que estas poseen. El mismo recorre los diferentes estamentos de la planta baja donde se desarrollan actividades propias de este tipo establecimientos  El vehículo guía autónomo cuenta con los elementos necesarios para desplazarse en forma independiente sin colisionar con las instalaciones u ocasionales transeúntes.


## 2) Los materiales utilizados en este proyecto son:

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

## 3) Armado del prototipo
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

## 4) Software Utilizado

### 4-1 Grabado del software en la tarjeta micro SD

En primera instancia formateamos la memoria con SD Formater mediante el adaptador de memoria enchufado a un puerto USB de la PC:

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/Configuraci%C3%B3n%20de%20la%20MSD%202%20github.jpg)

Luego utilizamos USB Image Tool para grabar la imagen del sistema que utilizará el robot mediante el adaptador USB de memoria enchufado a un puerto USB de la PC :

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/USB%20Image%20Tool%20github.jpg)

### 4-2 Armado de la máquina virtual con Ubuntu 18.04 y Jupiter para  trabajar con el código que utilizará el robot.

Cabe destacar que tanto Jetson Nano como Blackberry utilizan el sistema operativo Linux por lo que es necesario contar con una máquina que utilice este SO.  Si bien hay diversas manera de obtener una máquina vbrtual entre las que podemos citar la utilización de software específico para realizar la virtualización como VMware, VirtualBox y otros, tambien se podría utilizar dual boot en la PC para seleccionar un arranque con Linux, en este caso uitlizaremos la posibilidad que nos brinda Windows 10 de ejecutar una terminal de Ubuntu como una aplicación.

Inicialmente debemos ener actualizado Windos 10 e instalar el Subsistema de Windows para Linux con:

dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

Luego debemos habilitar la característica opcional Plataforma de máquina virtual en Windos ejecutando en el power Shell el comando:

dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

para luego descargar el paquete de Linux, Ubuntu 18.04 LTS

Tendeemos de ese modo Ubuntu 18.04 en el escritorio de windows con un acceso que se verá de la siguiente manera

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/icono%20ubuntu.jpg)

Accedemos a Ubuntu 18.04 

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/ubuntu%2018.04.jpg)

### 4-3 Instaalción de Jupiter en Ubuntu 18.04:

Actualizamos el índice de paquetes local apt 

$ sudo apt update

Luego descargamos e instalaremos los paquetes
Instalamos pip y los archivos de encabezado de Python, utilizados por algunas dependencias de Jupyter:

sudo apt install python3-pip python3-dev

Creamos un entorno virtual de Python para administrar nuestros proyectos e instalaremos Jupyter en este entorno virtual.

$ sudo -H pip3 install --upgrade pip


$ sudo -H pip3 install virtualenv

Creamos un directorio en el que podamos guardar los archivos de nuestro proyecto e ingresamos en él

$ mkdir ~/miproyecto

$ cd ~/miproyecto

Creamos un entorno virtual de Python dentro del directorio miproyecto

Activamoe el entorno virtual para instalar Jupiter

$ source miproyecto_env/bin/activate

Instalamos jupyter

$ pip install jupyter

Finalmente ejecutamos jupyter

$ jupyter notebook

Nos saldrá una notificación como la siguiente, por lo que usamos estas direcciones para ejecutarla en un navegador

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/ejecutando%20jupyter.jpg)

Y se mostrará jupyter para poder trabajar con el código de nuestro vehículo guía experimental

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/jupyter.jpg)

## 5) Inicio del trabajo con el código del vehículo

Utilizamos en este proyecto la biblioteca Donkey Car por lo que en todos los casos en necesario importarla

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/codigo%20vehiculo.JPG)

### 5-1 Repositorio de datos

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/repositorio%20de%20datos.JPG)

### 5-2 Tensorflow - Keras

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/keras%20c%C3%B3digo.JPG)


### 5-3 Crear carpeta de datos

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/crear%20carpeta%20de%20datos.JPG)

### 5-4 Administrar carpeta de datos

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/carpeta%20de%20datos.JPG)

## 6) Conducir y entrenar el modelo

![myimage-alt-tag](https://github.com/NorbertoAramayo/archivosnuevos/blob/main/entrenar%20el%20modelo.JPG)






















































