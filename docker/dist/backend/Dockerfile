FROM php:7.4-rc-fpm-alpine

#   |--------------------------------------------------------------------------
#   | Application
#   |--------------------------------------------------------------------------

COPY . /var/www/html

RUN chmod -R 777 /var/www/html/storage/logs
RUN chmod -R 777 /var/www/html/storage/framework
RUN chmod -R 777 /var/www/html/bootstrap/cache
