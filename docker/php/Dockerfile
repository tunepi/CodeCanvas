FROM php:8.3.19-fpm-alpine3.21

# install composer
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer

# install packages
RUN apk update
RUN apk add git nodejs npm bash

# install php extensions
RUN docker-php-ext-install pdo pdo_mysql