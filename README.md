# how-to-setup-php-project-in-docker
create docker-compose.yml file with content

version: '3.8'
services:
  php-apache-environment:
    container_name: php-apache
    image: php:8.0-apache
    volumes:
      - ./php/src:/var/www/html/
    ports:
      - 8000:80

create a index file under /php/src folder

run command on cmd
docker-compose up


open browser
http://localhost:8000/
