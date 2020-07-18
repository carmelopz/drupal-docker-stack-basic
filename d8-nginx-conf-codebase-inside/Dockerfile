FROM nginx:1.19.1
COPY ./server.conf   /etc/nginx/nginx.conf
COPY ./site.conf   /etc/nginx/conf.d/default.conf
COPY ../src/   /var/www/html
COPY ../settings/settings.local.php   /var/www/html/web/sites/default/settings.local.php
