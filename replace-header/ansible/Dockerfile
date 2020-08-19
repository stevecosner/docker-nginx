#Build and run the Nginx Docker container and use replace cmd with mariadb server to update the header.

FROM nginx:latest

MAINTAINER steve

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install mariadb-server -y
RUN replace RUN replace "Welcome to nginx!" "Nginx on Docker" -- /usr/share/nginx/html/index.html "Welcome to Nginx on Docker" -- /usr/share/nginx/html/index.html

