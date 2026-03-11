# 
FROM ubuntu:22.04

LABEL AUTOR="Franco Sergio Peryra"

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
  apt-get install -y --no-install-recommends apache2 php libapache2-mod-php php-mysql && \
  rm -rf /var/lib/apt/lists/* 
  
EXPOSE 80

ENTRYPOINT ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]

    