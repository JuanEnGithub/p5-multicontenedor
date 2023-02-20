
### Guestbook

Creamos imagen


docker-compose up -d


Abrimos el contenedor

archivo yml


version: '3.1'
services:
  app:
    container_name: guestbook-compose
    image: iesgn/guestbook
    restart: always
    ports:
      - 80:5000
  db:
    container_name: redis-compose
    image: redis
    restart: always
