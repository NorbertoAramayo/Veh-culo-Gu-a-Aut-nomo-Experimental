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
Se describe en este apartado el armado del prototipo del robot guía, destacando sus partes mas importantes como el armado de la computadora Jetson Nano, los conectores a los diferentes periféricos de la misma, los elementos para la comunicacion Wifi del robot, los efectores, los actuadores, y los sensores utilizados (en este caso una cámara web Raspberry según lo detallado en la lista de elementos de la sección anterior).
[Se describe aquí el armado del prototipo](https://github.com/NorbertoAramayo/Prototipo/blob/main/README.md)[...]

## 4) Software Utilizado
Se muestra en esta sección la preparación de la tarjeta MSD que se utiliza en el robot guía experimental, el software utilizado y su utilización. 
Si bien puede utilizarse una tarjeta de 16 GB, es recoomendable una de mayor capcidad a los efectos de realizar las tareas de administración que se necesitan
teiendo en cuenta también que en la misma estará el SO que utilizará el robot experimental y donde correrá la terminal de Ubuntu a los efectos qeu fueran necsarios.
[MSD- Instalación y Configuración]()[...]

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






















































