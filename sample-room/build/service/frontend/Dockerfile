FROM php:8.2-apache
WORKDIR /var/www/html

COPY index.php /var/www/html/index.php
COPY flag.txt /var/www/html/flag.txt

RUN apt-get update && \
    apt-get install -y \
    nmap && \
    rm -rf /var/lib/apt/lists/*

EXPOSE 80

RUN usermod -aG root www-data
