FROM nginx

MAINTAINER steve

RUN mv /usr/share/nginx/html/index.html /usr/share/nginx/html/backupindex.html
RUN mv /usr/share/nginx/html/50x.html /usr/share/nginx/html/backup50x.html
RUN apt update
RUN apt install git -y
RUN git clone https://github.com/BlackrockDigital/startbootstrap-landing-page.git
RUN cp -r startbootstrap-landing-page/. /usr/share/nginx/html

