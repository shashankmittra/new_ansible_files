FROM ubuntu:18.10 as builder
WORKDIR /root/
COPY test.txt /root/
EXPOSE 80

FROM httpd:2.4
COPY index.html /usr/local/apache2/htdocs/

WORKDIR /root/
