# Nifi-ELK

####1
#####Creamos un docker-compose file con Nifi y ELK

[Docker-compose](https://github.com/lggx/Nifi-ELK/blob/main/docker-compose.yml "Docker-compose")

####2
#####Creamos el siguiente flow de Nifi. 

[Nifi Templeate](https://github.com/lggx/Nifi-ELK/blob/main/data311.xml "Nifi Templeate")

<img src="https://github.com/lggx/Nifi-ELK/blob/main/nifi.png" width="1000"/>

####3
#####Con el templeate anterior se ha creado un indice con el nombre "crime". Ejecutamos el dev tool el codigo que vemos en la imagen para crear un nuevo indice donde el dato de la localizacion es del tipo geo_point

<img src="https://github.com/lggx/Nifi-ELK/blob/main/dev%20tools.png" width="1000"/>

####4
#####
