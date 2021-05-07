# CURSO SYMFONY 5

## Introducción

- [Instalación de symfony, creación nuevo proyecto, integración con git, permisos de ficheros, servidor integrado de php, controlador único](./instalacion.md)
- [Estructura de un proyecto symfony](./estructura_directorios.md)
- [Patrón MVC](./mvc.md)

## Creación de la página de Home y menú público

- [Introducción a Controllers](./controllers_intro.md)
- [Introducción al Routing](./routing_intro.md)
- [Introducción a Twig](./twig_intro.md)
- Ejercicio: Crear varias páginas enlazadas con un menú


## Introducción al profiler y a los entornos

## Twig

- Variables. Acceso a atributos con (.)
- Variables globales
- set
- filtros
- funciones
- Named arguments
- Estructuras de control (if, for…)
- Comentarios
- include
- extends y block
- html escaping
- Operadores

https://twig.symfony.com/doc/3.x/templates.html

## Acceso a base de datos. Doctrine.

- Entidades simples
- Entity Manager
- Repository
- Entidades relacionadas
- DQL y Query Builder
- Native SQL
- Ingeniería inversa
- ArrayCollection
- El problema de las N+1 queries

## Instalación de Bundles

- Fixtures (Sin bundle y con NelmioAliceBundle)

## Controladores

- El objeto Response
- El objeto Request
- Creación de otras páginas de la zona pública
- Routing avanzado

## Internacionalización (i18n)

- Extracción de contenidos traducibles y actualización automática de los catálogos
- Depuración de traducciones

## Servicios

- El contenedor de servicios y la inyección de dependencias
- Parameters
- Configuración avanzada de servicios
- Entornos y variables de entorno.
- Archivos de configuración de symfony. 

## El componente Security

- Autenticación
- Autorización. Roles.
- Voters
- El bundle FOSUserBundle


## Caché

## Logs

- Cómo logear mensajes en diferentes ubicaciones
- Manejadores de logs nativos
- Cómo rotar los ficheros de log
- Cómo utilizar un blog en un servicio
- Añadir datos extra a los mensajes de log

## La consola de symfony

- Comandos predefinidos.
- Creación de comandos de consola personalizados.

## Formularios

- Formularios y validaciones. Mensajes Flash.
- Eventos de formulario
- Formulario dinámico basado en los propios datos del formulario
- Formulario dinámico basado en el usuario
- Temas personalizados
- Validaciones personalizadas

## Envío de correos

## Eventos

- El Event Dispatcher
- Eventos personalizados
- Listeners y Subscribers
- Eventos del Kernel de Symfony

## Creación de APIs REST con Symfony

- JsonResponse
- LexitJwtBundle

## El serializer de symfony

- Cómo manejar referencias circulares
- Cómo manejar la profundidad de la serialización
- Normalizers
- Encoders
- Cómo configurar qué atributos se serializan
- Cómo convertir nombres de propiedades al serializar y des-serializar 

## Componente Workflow

## Gestión de recursos CSS y JavaScript

- Manejo de archivos Sass y Less
- Source Maps
- Manejo de archivos TypeScript
- Versionado de assets
- Cómo pasar información de Twig a JavaScript

## Testing automatizado

## Twig Avanzado

- Cómo generar otros formatos de salida (css, javascript, xml…)
- Cómo inyectar variables globales
- Sobreescribir plantillas de bundles de terceros
- Crear plantillas sin controladores
- Cómo crear una extensión de twig

## Depuración en Symfony. El profiler

- Cómo crear un Data Collector personalizado
- Cómo acceder a los datos del profiler programáticamente
- Cómo utilizar Matchers para activar o desactivar el profiler programáticamente
- Cómo cambiar la ubicación del Profiler Storage

## Flex

- Recipes
- Creación de bundles
- Extensión de bundles
 
## Deploy y rendimiento
