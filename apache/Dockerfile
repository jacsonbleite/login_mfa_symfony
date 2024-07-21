FROM php:8.3-apache

RUN apt-get update && apt-get install -y \
    libpq-dev \
    && docker-php-ext-install pdo pdo_pgsql

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

WORKDIR /var/www/html

# Configuração adicional do Apache
COPY ./000-default.conf /etc/apache2/sites-available/000-default.conf

RUN a2enmod rewrite
