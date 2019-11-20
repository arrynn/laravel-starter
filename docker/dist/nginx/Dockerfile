FROM nginx:1.17-alpine

#   |--------------------------------------------------------------------------
#   | Application config
#   |--------------------------------------------------------------------------

COPY ./docker/dev/nginx/default.conf /etc/nginx/conf.d/default.conf

#   |--------------------------------------------------------------------------
#   | Application config
#   |--------------------------------------------------------------------------

COPY . /var/www/html

RUN chmod -R 777 /var/www/html/storage/logs
RUN chmod -R 777 /var/www/html/storage/framework
RUN chmod -R 777 /var/www/html/bootstrap/cache
