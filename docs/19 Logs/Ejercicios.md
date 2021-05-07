Ejercicios
==========

Ejercicio 19.1
--------------

Asocia cada manejador con su comportamiento: 

Manejadores:

1) group
2) fingers_crossed
3) rotating_file
4) deduplicaded


Comportamientos:

A) Genera ficheros de log rotativos.

B) Guarda en memoria todos los mensajes de log, sean del nivel que sean, y si en algún momento de la petición alguno de los mensajes alcanza al menos el nivel indicado en *action_level*, entonces envia TODOS los logs a otro manejador.

C) Elimina los mensajes repetidos durante el periodo de tiempo especificado y se los pasa a otro manejador

D) Hace que los mensajes de log sean manejados por más de un handler


Respuestas:

1 - D
2 - B
3 - A
4 - C



 
Peso de los ejercicios:
Tema 17: 50%
Tema 18: 40%
Tema 19: 10%