FROM nginx

MAINTAINER steve

RUN mv /usr/share/nginx/html/index.html /usr/share/nginx/html/backupindex.html
RUN mv /usr/share/nginx/html/50x.html /usr/share/nginx/html/backup50x.html
RUN apt update
RUN apt install git -y
RUN git clone https://github.com/stevecosner/bootstrap-starter.git
RUN cp -r bootstrap-starter/. /usr/share/nginx/html

