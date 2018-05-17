# Practica MongoDB

Pr�ctica para la asignatura de base de datos

## Ejercicio 1

Crear una base de datos

En MongoDB no existe ning�n comando estilo CREATE DATABASE, ni nada as�, lo que hace mongodb es crear una colecci�n (base de datos) en el momento que se le inserta un objeto o documento (registro de una tabla por llamarlo de alguna forma) a dicha colecci�n.
He creado la base de datos con el comando use practicaMongoDB y luego he usado el comando db para comprobar que me encuentro en la base de datos que acabo de crear:

<img src="Capturas/1.PNG">

## Ejercicio 2

Tener una colecci�n

Para ver las colecciones que tengo hay que usar el comando <em>show collections</em>:

<img src="Capturas/2.PNG">


## Ejercicio 3

Insertar, modificar y borrar documentos en la colecci�n

Para insertar documentos dentro de la colecci�n, primero tenemos que a�adirlos, por ejemplo pel�culas, se a�aden de la siguiente manera:

<img src="Capturas/3.PNG">

Ahora esos objetos que hemos creado los tenemos que insertar en una colecci�n, por ejemplo en <em>listaPeliculas</em>:

<img src="Capturas/4.PNG">

Para visualizar lo que hay dentro de la colecci�n lo he hecho de la siguiente manera:

<img src="Capturas/5.PNG">

Para visualizar solo un documento de la colecci�n:

<img src="Capturas/6.PNG">

Hay varias formas para modificar un documento de una colecci�n con MongoDB, el que yo he usado ha sido UPDATE() y $SET

Voy a modificar el a�o de la pel�cula La gran belleza

<img src="Capturas/7.PNG">

Aqu� podemos comprobar que el a�o se la pel�cula se ha modificado correctamente

<img src="Capturas/8.PNG">

Para eliminar un documento hay que usar los siguientes comandos, lo que he hecho despu�s de eliminar es mostrar un listado de la colecci�n para comprobar que se ha borrado correctamente la pel�cula3 cuyo autor es Carlos Vermut:

<img src="Capturas/9.PNG">

## Ejercicio 4

Crea un �ndice sobre un campo de la colecci�n

Para crear un �ndice hay que usar el siguiente comando:

<img src="Capturas/10.PNG">

## Ejercicio 5

Realizar consultas en las que utilices, igual, mayor y menor que.

Para estas consultas tengo que insertar  m�s documentos, en este caso he utilizado la consulta para insertar varios elementos juntos en la colecci�n:

<img src="Capturas/11.PNG">

Esta consulta es para mostrar las pel�culas que se hayan lanzado en 2014, (usando el operador de igual que):

<img src="Capturas/12.PNG">

Esta consulta es para mostrar las pel�culas a partir de 1960 (usando el operador de mayor que):

<img src="Capturas/13.PNG">

Esta consulta es para mostrar las pel�culas lanzadas antes de 1950 (usando el operador de menor que):

<img src="Capturas/14.PNG">

## Ejercicio 6

Realizar una consulta en la que los documentos aparezcan ordenados y se l�mite el n�mero de estos mostrados:

Para mostrar los documentos ordenador se utiliza el 1 para ordenarlos en orden ascendente y el -1 para ordenarlos en orden descendente.

Lo que voy hacer es ordenar las 5 primeras pel�culas por t�tulo en orden ascendente:

<img src="Capturas/15.PNG">

## Ejercicio 7

Realizar una consulta con agrupamiento y una funci�n para mostrar la media, o suma, o la que t� decidas.

Para hacer la consulta con la funci�n de la media que es la que he elegido, le he tenido que a�adir el dato de n�mero de espectadores

<img src="Capturas/16.PNG">

En la siguiente consulta he agrupado las pel�culas por a�o:

<img src="Capturas/17.PNG">

Luego he comprobado si hay pel�culas repetidas en el mismo a�o, en la siguiente captura podemos comprobar que en el a�o 2014 hay 2 pel�culas:

<img src="Capturas/18.PNG">

Y por �ltimo he hecho la media del n�mero de espectadores de cada a�o:

<img src="Capturas/19.PNG">

















