# Configuración de servidor PAVCO

Pasos realizados para configurar el servicio.

## Acceso
- se crea una instancia de Ubuntu 16.04 y se accede por SSH
- se da de alta un usuario en sistema y se añade al grupo sudo para que pueda ejecutar comandos de root

## Servicios
- se instala Apache, MySQL y Git 
- se instala Composer, se configura el repositorio Git y se hace push al código de Laravel

## Repositorio
- Repositorio GIT: se crea un directorio para usarlo como repositorio con: `git init --bare`. En el subdirectorio hooks se añade un archivo post-receive y se le dan permisos de ejecución con los directorios apropiados:

`git --work-tree=/var/www/html  --git-dir=/home/demo/repositorio.git checkout -f`

## Permisos
- se asignan permisos adecuados a las carpetas de storage y de cache de Laravel

```
sudo chgrp -R www-data storage bootstrap/cache
sudo chmod -R ug+rwx storage bootstrap/cache
```

## Base de datos
- se verifica la conexión a la base de datos y se crea una base para el proyecto

## API key
- se genera una llave única para Laravel

## Migraciones
- se ejecutan las migraciones

## Apache
- se configura  el acceso al directorio correctamente en Apache para acceder vía web a la app Laravel. DocumentRoot debe apuntar a /var/www/html/public.

## Colaboración
- se añaden llaves ssh de los usuarios que vayan a colaborar en el código vía larval
