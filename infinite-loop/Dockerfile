FROM nginx

MAINTAINER steve

RUN mv /usr/share/nginx/html/index.html /usr/share/nginx/html/backupindex.html
RUN mv /usr/share/nginx/html/50x.html /usr/share/nginx/html/backup50x.html
RUN apt update
ADD web /usr/share/nginx/html
#RUN cp -r web/. /usr/share/nginx/html
