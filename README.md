# apache-modes
Descripción de tipos de instalación apache

### Apache prefork

Es el modelo tradicional por defecto de la instalación de apache el cual utiliza `mod_php` el cual consume muchos recursos del servidor ya que utiliza muchos procesos para poder soportar una cantidad de visitas considerable.

> Por ejemplo un request de laravel sin cache puede tomar entre 10 y 25 MB por proceso

### Apache worker

Es el modelo basado en threads y utiliza la versión `php_fpm` la cual soporta la diferentes hilos en un mismo proceso y por lo tanto es thread safe.

> Por ejemplo un request de laravel sin cache puede tomar entre 1 y 3 MB por proceso

#### Configuración y trucos
> TODO
