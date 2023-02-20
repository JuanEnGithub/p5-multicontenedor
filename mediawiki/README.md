

### Mediawiki 

Desplegamos el contenedor


docker-compose up -d


Abrimos el contenedor


docker-compose:

version: '3.2'
services:
  web:
    image: mediawiki
    ports:
      - 80:80
    volumes:
      - database:/var/www/data
      - images:/var/www/html/images
volumes:
    database:
    images:
