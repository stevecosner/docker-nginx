# docker-nginx-php
Create a web server and test php config with phpinfo page using the nginx docker container image.

Using php7.0-fpm

Clone repo.

cd docker-nginx-php

docker build -t nginx-php-1 .

docker run -d -p 80:80 nginx-php-1

docker exec <CONTAINERNAME> service php7.0-fpm start

Open browser to hostname or docker container ip and test connnection of webserver as well as php connection.


