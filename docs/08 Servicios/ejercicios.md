Ejercicio 8.1
-------------

Enunciado: ¿Cómo configurarías el fichero services.yaml para que la aplicación se comporte como sigue?

- Que los Repositorios y los Formularios no se consideren servicios
- Que haya que registrar los servicios especiales que requieren especificar una tag, como commandos, subscribers, extensiones de twig, etc.

Subir un fichero de texto con el contenido del fichero services.yaml


Ejercicio 8.2
-------------

Condidera el enunciado completo de la práctica final. 

NOTA: Se considerará en este ejercicio que donde diga "... los estados de XXXXXXX se deben gestionar con el componente Workflow ..." dice "... los estados de XXXXXXX se deben gestionar con un servicio ...".

Analizar el enunciado de la práctica final y diseñar los servicios que se consideren necesarios.

NOTA: Se recomienda realizar este ejercicio en el proyecto en el que se vaya a realizar la práctica final, para aprovechar el trabajo.

Tareas: 
- Crea un directorio Services/ dentro del directorio src/.
- En dicho directorio, crea todos los servicios que crearías para este proyecto. Un archivo por cada servicio.
- Implementa el esqueleto de cada servicio. Es decir:
  - Comentario con descripción del servicio
  - Constructor con sus argumentos
  - Métodos del servicio con sus argumentos. 
  - Sobre cada método, comentario con: la utilidad del método, argumentos de entrada y qué es lo que retorna la función.
  - NO HAY QUE PROGRAMAR el contenido de ningún métdodo. Los métodos se deben dejar vacíos.

Subir un fichero zip con el contenido de la carpeta Services.

Ejemplo:

Archivo src/Services/EmailManager.php
```php
/**
* Servicio que gestiona el envío de correo
*
*/
class EmailManager {
	
	/**
	* Envía un correo a los comerciales con la 
	* información de la nueva solicitud
	*
	* Devuelve true si todo ha ido bien o false si 
	* no se ha podido enviar el correo
	*/
	public function enviarCorreosSolicitudPresupuestoAComerciales(SolicitudPresupuesto $solicitud): boolean {

	}

	/**
	* Envía un correo al solicitante del presupuesto indicando  
	* que se ha recibido la solicitud
	*
	* Devuelve true si todo ha ido bien o false si 
	* no se ha podido enviar el correo
	*/
	public function enviarCorreosSolicitudPresupuestoASolicitante(SolicitudPresupuesto $solicitud): boolean {

	}

	/**
	* Envía un correo al solicitante del presupuesto
	* indicando que se ha aprobado el presupuesto
	*
	* Devuelve true si todo ha ido bien o false si 
	* no se ha podido enviar el correo
	*/
	public function enviarCorreosPresupuestoAprobado(SolicitudPresupuesto $solicitud): boolean {

	}

	...........
}
```



