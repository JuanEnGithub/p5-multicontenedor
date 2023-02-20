
### Adminer 🔧

Comando para desplegar contenedor


docker-compose up -d


Abrimos el contenedor



usuario: root
contraseña: example


archivo yml



version: '3.1'

services:

  adminer:
    image: adminer
    restart: always
    ports:
      - 8080:8080

  db:
    image: mysql:5.6
    restart: always
    environment:
      MYSQL_ROOT_PASSWORD: example
