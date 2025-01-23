FROM php:8.3-fpm

# Install system dependencies
RUN apt-get update && apt-get install -y git curl zip unzip nano libzip-dev

# Install PHP extensions
RUN docker-php-ext-install pdo_mysql

# Install PHP extensions
RUN docker-php-ext-install zip

# Get latest Composer
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

WORKDIR /var/www
