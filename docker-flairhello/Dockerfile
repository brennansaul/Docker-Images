FROM resin/raspberry-pi-alpine-node
MAINTAINER brennansaul jamessaul7629@gmail.com

RUN apk update

RUN apk add nginx php5-fpm 

RUN mkdir -p /run/nginx

ADD www /www
ADD nginx.conf /etc/nginx/
ADD php-fpm.conf /etc/php5/php-fpm.conf
ADD run.sh /run.sh

ENV LISTEN_PORT=80

EXPOSE 80
CMD /run.sh
