FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install tzdata -y
RUN apt-get install nginx -y
RUN apt-get install php -y
RUN apt-get install php-fpm -y
RUN mv /usr/share/nginx/html/index.html /usr/share/nginx/html/index.main
ADD index.html /usr/share/nginx/html
RUN mv /etc/nginx/sites-available/default /etc/nginx/sites-available/default.main
ADD default /etc/nginx/sites-available/
ADD info.php /usr/share/nginx/html
RUN mv  /etc/php/7.2/fpm/php.ini  /etc/php/7.2/fpm/php.ini.backup
ADD php.ini /etc/php/7.2/fpm/
RUN mv /etc/php/7.2/fpm/pool.d/www.conf /etc/php/7.2/fpm/pool.d/www.conf.backup
ADD www.conf /etc/php/7.2/fpm/pool.d/

