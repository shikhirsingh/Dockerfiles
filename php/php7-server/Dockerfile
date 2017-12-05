FROM php:7.2-apache
RUN apt-get update && apt-get install -y wget 
WORKDIR /usr/local/etc/php/
RUN wget https://raw.githubusercontent.com/php/php-src/8305a73483e854f314b8afa2d65dbcb0e7fae1b9/php.ini-development
RUN mv php.ini-development php.ini
WORKDIR /var/www/html/

