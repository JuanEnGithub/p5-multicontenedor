
### Apache

Creamos el contenedor

docker-compose up -d


Ejecutamos el contenedor


docker-compose:

version: '3.1'
services:
  apache:
    image: httpd:latest
    container_name: my-apache-app
    ports:
    - '8080:80'
    volumes:
    - ./website:/usr/local/apache2/htdocs
