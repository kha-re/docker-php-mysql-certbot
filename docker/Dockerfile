FROM php:8.3-fpm

RUN apt-get update && apt-get install -y \
    git \
    curl \
    zip \
    unzip \ 
    nano \
    libzip-dev \
    && docker-php-ext-install zip

WORKDIR /var/www