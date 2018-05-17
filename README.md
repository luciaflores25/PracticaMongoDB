# Practica MongoDB

Práctica para la asignatura de base de datos

## Ejercicio 1

Crear una base de datos

En MongoDB no existe ningún comando estilo CREATE DATABASE, ni nada así, lo que hace mongodb es crear una colección (base de datos) en el momento que se le inserta un objeto o documento (registro de una tabla por llamarlo de alguna forma) a dicha colección.
He creado la base de datos con el comando use practicaMongoDB y luego he usado el comando db para comprobar que me encuentro en la base de datos que acabo de crear:

<img src="Capturas/1.PNG">

## Ejercicio 2

Tener una colección

Para ver las colecciones que tengo hay que usar el comando <em>show collections</em>:

<img src="Capturas/2.PNG">


## Ejercicio 3

Insertar, modificar y borrar documentos en la colección

Para insertar documentos dentro de la colección, primero tenemos que añadirlos, por ejemplo películas, se añaden de la siguiente manera:

<img src="Capturas/3.PNG">

Ahora esos objetos que hemos creado los tenemos que insertar en una colección, por ejemplo en <em>listaPeliculas</em>:

<img src="Capturas/4.PNG">

Para visualizar lo que hay dentro de la colección lo he hecho de la siguiente manera:

<img src="Capturas/5.PNG">

Para visualizar solo un documento de la colección:

<img src="Capturas/6.PNG">

Hay varias formas para modificar un documento de una colección con MongoDB, el que yo he usado ha sido UPDATE() y $SET

Voy a modificar el año de la película La gran belleza

<img src="Capturas/7.PNG">

Aquí podemos comprobar que el año se la película se ha modificado correctamente

<img src="Capturas/8.PNG">

Para eliminar un documento hay que usar los siguientes comandos, lo que he hecho después de eliminar es mostrar un listado de la colección para comprobar que se ha borrado correctamente la película3 cuyo autor es Carlos Vermut:

<img src="Capturas/9.PNG">

## Ejercicio 4

Crea un índice sobre un campo de la colección

Para crear un índice hay que usar el siguiente comando:

<img src="Capturas/10.PNG">

## Ejercicio 5

Realizar consultas en las que utilices, igual, mayor y menor que.

Para estas consultas tengo que insertar  más documentos, en este caso he utilizado la consulta para insertar varios elementos juntos en la colección:

<img src="Capturas/11.PNG">

Esta consulta es para mostrar las películas que se hayan lanzado en 2014, (usando el operador de igual que):

<img src="Capturas/12.PNG">

Esta consulta es para mostrar las películas a partir de 1960 (usando el operador de mayor que):

<img src="Capturas/13.PNG">

Esta consulta es para mostrar las películas lanzadas antes de 1950 (usando el operador de menor que):

<img src="Capturas/14.PNG">

## Ejercicio 6

Realizar una consulta en la que los documentos aparezcan ordenados y se límite el número de estos mostrados:

Para mostrar los documentos ordenador se utiliza el 1 para ordenarlos en orden ascendente y el -1 para ordenarlos en orden descendente.

Lo que voy hacer es ordenar las 5 primeras películas por título en orden ascendente:

<img src="Capturas/15.PNG">

## Ejercicio 7

Realizar una consulta con agrupamiento y una función para mostrar la media, o suma, o la que tú decidas.

Para hacer la consulta con la función de la media que es la que he elegido, le he tenido que añadir el dato de número de espectadores

<img src="Capturas/16.PNG">

En la siguiente consulta he agrupado las películas por año:

<img src="Capturas/17.PNG">

Luego he comprobado si hay películas repetidas en el mismo año, en la siguiente captura podemos comprobar que en el año 2014 hay 2 películas:

<img src="Capturas/18.PNG">

Y por último he hecho la media del número de espectadores de cada año:

<img src="Capturas/19.PNG">

















