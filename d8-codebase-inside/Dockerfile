image: php:7.4.8-fpm-buster
COPY ./nginx/server.conf   /etc/nginx/nginx.conf
COPY ./nginx/site.conf   /etc/nginx/conf.d/default.conf
COPY ./src/   /var/www/html
COPY ./settings/settings.local.php   /var/www/html/web/sites/default/settings.local.php

ENV COMPOSER_ALLOW_SUPERUSER 1

RUN cd /var/www/html; composer install
