FROM php:7.4-rc-fpm-alpine

#   |--------------------------------------------------------------------------
#   | Composer
#   |--------------------------------------------------------------------------

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer

#   |--------------------------------------------------------------------------
#   | Xdebug
#   |--------------------------------------------------------------------------

RUN apk add --no-cache --virtual .build-deps $PHPIZE_DEPS \
    && pecl install xdebug \
    && docker-php-ext-enable xdebug \
    && apk del -f .build-deps

#   |--------------------------------------------------------------------------
#   | Application
#   |--------------------------------------------------------------------------

COPY . /var/www/html
