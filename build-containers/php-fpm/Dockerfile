FROM php:8.2-rc-fpm-buster

RUN docker-php-ext-install pdo_mysql

COPY php.ini /etc/php.ini
COPY php-fpm.conf /etc/php-fpm.comf
COPY php-fpm.d/www.conf /etc/php-fpm.d/www.conf