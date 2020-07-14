# https://gist.github.com/giansalex/2776a4206666d940d014792ab4700d80

# https://medium.com/@FernandoDebrand/criando-um-ambiente-de-desenvolvimento-php-com-docker-compose-a7cad3373df0


FROM php:7.4-apache

MAINTAINER Edson Linhares <edson_linhares@yahoo.com.br>

RUN apt-get update && apt-get install -y libgcrypt20-dev zlib1g-dev libpng-dev libicu-dev libbz2-dev libzip-dev libxml2-dev libldap2-dev
RUN docker-php-ext-install mysqli
RUN docker-php-ext-install -j$(nproc) gd
RUN docker-php-ext-install intl
RUN docker-php-ext-install ldap
RUN docker-php-ext-install opcache
RUN docker-php-ext-install bz2
RUN docker-php-ext-install zip
RUN docker-php-ext-install xmlrpc
RUN docker-php-ext-install exif
