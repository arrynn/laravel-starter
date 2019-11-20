FROM nginx:1.17-alpine

#   |--------------------------------------------------------------------------
#   | Application config
#   |--------------------------------------------------------------------------

COPY ./docker/dev/nginx/default.conf /etc/nginx/conf.d/default.conf

COPY . /var/www/html
