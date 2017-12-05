```
wget https://raw.githubusercontent.com/shikhirsingh/Dockerfiles/master/php/php7-server/Dockerfile
docker image build -t telesign-php:3.0 .
docker container run -d -p 80:80 --name my-apache-php-app -v "$PWD":/var/www/html telesign-php:3.0
docker run --rm --name=composer -v $(pwd):/www matriphe/alpine-composer:latest composer require telesign/telesign
wget https://raw.githubusercontent.com/TeleSign/php_telesign/master/examples/messaging/1_send_message.php
```
