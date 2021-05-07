Ejercicios
==========

Ejercicio 9.1
-------------

Enunciado: 

Imaginemos que nuestra aplicación symfony consiste únicamente de una API REST.

Tenemos también un servicio TokenValidatorService con un método validate($token) que nos devuelve un booleano indicando si un token es válido o no para acceder a la API.

En nuestro services.yaml tenemos activados autoconfigure y autowire.

Crear y configurar un subscriber que lance un AccessDeniedHttpException si se realiza una petición a cualquier url de la API con un token que no sea válido.

Subir un fichero zip o tar.gz con los ficheros creados o modificados para este propósito.

NO es necesario programar el servicio TokenValidatorService.

Ejercicio 9.2
-------------

Enunciado: 

Igual que el ejercicio 9.1 pero con un listener en vez de con un subscriber.

Subir un fichero zip o tar.gz con los ficheros creados o modificados para este propósito.

NO es necesario programar el servicio TokenValidatorService.


Ejercicio 9.3
-------------


Programar un EventSuscriber que:

1) Cuando ocurra el evento 'onPresupuestoSolicitado', llame al método o métodos de envío de correo correspondientes definidos en los servicios del ejercicio 8.2

2) Cuando ocurra el evento 'onPresupuestoAprobado' llame al método o métodos de envío de correo correspondientes definidos en los servicios del ejercicio 8.2


Subir un fichero zip o tar.gz con los ficheros creados o modificados para este propósito.
