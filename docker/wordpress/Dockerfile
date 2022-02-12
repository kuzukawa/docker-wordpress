FROM wordpress:5.8.3-php7.4

RUN apt-get update \
    && pecl install xdebug \
    && docker-php-ext-enable xdebug

COPY ./docker/wordpress/xdebug.ini /usr/local/etc/php/conf.d/xdebug.ini
CMD ["apache2-foreground"]
