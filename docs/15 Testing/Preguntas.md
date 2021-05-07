Preguntas
=========

En el componente de testeo PHP Unit Bridge de Symfony, ¿cuál de los siguientes códigos serviría para realizar un click en el enlace "Haz click aquí"?


A) 

```php
$client = static::createClient();
$client->selectLink('Haz click aquí')->click();
```

B) 

```php
$client = static::createClient();
$crawler = $client->request('GET', '/homepage');
$crawler->selectLink('Haz click aquí')->click();

```

C) 

```php
$client = static::createClient();
$crawler = $client->request('GET', '/homepage');
$link = $crawler->selectLink('Haz click aquí')->link();
$client->click($link);
```

D) 

```php
$client = static::createClient();
$link = $client->selectLink('Haz click aquí')->link();
$client->click($link);
```


Solución: C