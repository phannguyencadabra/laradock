FROM php:5.5-fpm
RUN pecl install xdebug-2.5.5 && docker-php-ext-enable xdebug
RUN docker-php-ext-install pdo_mysql && docker-php-ext-enable pdo_mysql
RUN pecl install redis-2.2.3 && docker-php-ext-enable redis

CMD ["php-fpm"]

EXPOSE 9000