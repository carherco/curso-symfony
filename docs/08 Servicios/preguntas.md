Preguntas
=========

Enunciado: Une cada clave del fichero services.yaml con su significado


Claves:

-autoconfigure
-autowire
-public

Significados:

- Si está a true, Symfony averigua los tags de los servicios sin necesidad de configurarlos.
- Si está a true, permite obtener los servicios a través de $container->get()
- Si está a true, habilita la inyección de dependencias mediante el tipado de argumentos en los métodos constructores de los servicios


Solución:

autoconfigure: Si está a true, Symfony averigua los tags de los servicios sin necesidad de configurarlos.

autowire: Si está a true, habilita la inyección de dependencias mediante el tipado de argumentos en los métodos constructores de los servicios

public: Si está a true, permite obtener los servicios a través de $container->get()