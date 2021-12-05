FROM php:8.1-fpm

RUN docker-php-ext-install pdo_mysql

COPY ./conf.d/xdebug.ini /usr/local/etc/php/conf.d/xdebug.ini
COPY ./conf.d/error_reporting.ini /usr/local/etc/php/conf.d/error_reporting.ini
COPY ./conf.d/php_ini.ini /usr/local/etc/php/conf.d/php_ini.ini

# uncomment the following line the first time the image container is run
#RUN pecl install xdebug
RUN docker-php-ext-enable xdebug
