FROM php:7.4-apache

RUN apt-get update && apt-get install -y \
    git \
    unzip \
    vim

# xdebug インストール
RUN pecl install xdebug \
  && docker-php-ext-enable xdebug

WORKDIR /var/www/html
#CMD ["php", "-S", "0.0.0.0:8000", "-t", "/var/www"]