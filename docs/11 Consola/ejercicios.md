Ejercicios
==========

Ejercicio 11.1
--------------

Partiendo de la estructura de base de datos alumnos.sql.zip ya utilizada en otros ejercicios, crear un comando de consola personalizado que saque un listado de las notas medias de las asignaturas de un grado entre dos fechas dadas.

El comando se utilizaría de la siguiente manera:

bin/console informes:notas nombregrado fechainicio fechafin

Ejemplo:

bin/console informes:notas "Ingeniería de montes" 2016-09-01 2017-08-31

El informe debe de presentar el nombre de cada asignatura junto con la media de las notas de los alumnos en dicha asignatura entre las fechas dadas.


Subir un archivo zip con el proyecto exceptuando los directorios node_modules, var y vendor