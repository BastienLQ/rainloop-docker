FROM php:7-apache

RUN apt-get update && \
    apt-get install -y unzip && \
    curl -O http://repository.rainloop.net/v2/webmail/rainloop-latest.zip && \
    unzip rainloop-latest.zip && \
    rm rainloop-latest.zip && \
    chmod -R 777 /var/www/html/data && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

COPY php.ini /usr/local/etc/php/conf.d/php.ini

VOLUME /var/www/html/data
EXPOSE 80
