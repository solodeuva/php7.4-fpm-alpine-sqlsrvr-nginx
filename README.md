# php:7.4-fpm-alpine + sqlsrvr driver + nginx 

Este contenedor fue construido para una aplicación laravel pero puede utilizarse para otros fines.

---
# Prerrequisitos del ejemplo

- Laravel App

# Runing Containers

Situarse dentro de la carpeta de la aplicación laravel y copiar todos los archivos.

En linea de comanos construir la imagen base ```laravel``` que esta definida en el archivo ```docker-compose.yml```.

`docker-compose build app`

Al terminar ejecutar.
`docker-compose up -d`

#### Para despliegue en producción sustituir los archivos

Para el despliegue en producción se utilizará la imagen de docker ```composer:1.9.3``` para instalar las dependencias y se copiaran a la imagen de ```php7.4-fpm-alpine```.

