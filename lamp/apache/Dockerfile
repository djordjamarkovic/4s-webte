FROM httpd:2.4.46-alpine
#FROM bitnami/apache:latest
RUN apk update; \
    apk upgrade;

#COPY ./apache.conf /usr/local/apache2/conf/httpd.conf

COPY ./cert/ssl.crt /usr/local/apache2/cert/certificate.crt
COPY ./cert/ssl.key /usr/local/apache2/cert/private.key
#RUN mkdir -p /var/run/apache2/

EXPOSE 80
EXPOSE 443


