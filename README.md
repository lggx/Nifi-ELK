# Nifi-ELK


#### Creamos un docker-compose file con Nifi y ELK

[Docker-compose](https://github.com/lggx/Nifi-ELK/blob/main/docker-compose.yml "Docker-compose")

#### Creamos el siguiente flow de Nifi. 
Se descagan los datos de la API con invokehttp, dividimos el Json con SplitJson y los cargamos a elsaticsearch con el PutElasticsearchHttp.

[Nifi Templeate](https://github.com/lggx/Nifi-ELK/blob/main/data311.xml "Nifi Templeate")

<img src="https://github.com/lggx/Nifi-ELK/blob/main/nifi.png" width="1000"/>

#### Cambiamos los datos de localizacion a geo_points para poder crear el mapa
Con el templeate anterior se ha creado un indice con el nombre "crime". Ejecutamos el dev tool el codigo que vemos en la imagen para crear un nuevo indice donde el dato de la localizacion es del tipo geo_point. 
Por ultimo pasamos los datos de un indice a otro. 

<img src="https://github.com/lggx/Nifi-ELK/blob/main/dev%20tools.png" width="1000"/>

#### Creamos el mapa

<img src="https://github.com/lggx/Nifi-ELK/blob/main/mapa.png" width="1000"/>

Tambien podemos extraer mas informacion de estos datos.

<img src="https://github.com/lggx/Nifi-ELK/blob/main/dashboard.png" width="1000"/>
