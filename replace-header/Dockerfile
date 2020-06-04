#Build and run the Nginx Docker container and use replace cmd with mysql server to update the header.

FROM nginx

MAINTAINER steve

RUN apt-get update
RUN apt-get install mysql-server -y
RUN replace "Welcome to nginx!" "Docker Nginx Test!" -- /usr/share/nginx/html/index.html
