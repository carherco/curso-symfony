Soluciones
==========

Ejercicio 4.1
-------------

/articles/es/2010/my-post
/articles/fr/2010/my-post.rss
/articles/es/2013/my-latest-post.html


Enviar fichero de texto con la definición de la ruta en formato anotación y en formato yaml.



```yml
article_show:
  path:     /articles/{_locale}/{year}/{slug}.{_format}
  defaults: { _controller: App\Controller\Article:show, _format: html }
  requirements:
      _locale:  en|fr
      _format:  html|rss
      year:     \d+
```

```php
class ArticleController extends Controller
{
    /**
     * @Route(
     *     "/articles/{_locale}/{year}/{slug}.{_format}",
     *     defaults={"_format": "html"},
     *     requirements={
     *         "_locale": "en|fr",
     *         "_format": "html|rss",
     *         "year": "\d+"
     *     }
     * )
     */
    public function showAction($_locale, $year, $slug)
    {
    }
}
```





Ejercicio 4.2:
--------------

Crear una acción y una ruta (con anotaciones en la acción) que redireccione todas las URLs acabadas en '/' a la misma URL sin la '/'.

Enviar un fichero de texto con la acción completa (anotaciones y código).


Ayuda: 
Una redirección en el controlador se realizar como sigue:
return $this->redirect($url);






```php
// src/Controller/RedirectingController.php
namespace App\Controller;

use Symfony\Bundle\FrameworkBundle\Controller\Controller;
use Symfony\Component\HttpFoundation\Request;

class RedirectingController extends Controller
{
    /**
     * @Route("/{url}", name="remove_trailing_slash",
     *     requirements={"url" = ".*\/$"})
     */
    public function removeTrailingSlash(Request $request)
    {
        $pathInfo = $request->getPathInfo();
        $requestUri = $request->getRequestUri();

        $url = str_replace($pathInfo, rtrim($pathInfo, ' /'), $requestUri);

        // 308 (Permanent Redirect) is similar to 301 (Moved Permanently) except
        // that it does not allow changing the request method (e.g. from POST to GET)
        return $this->redirect($url, 308);
    }
}
```
