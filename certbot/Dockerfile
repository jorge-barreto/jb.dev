FROM certbot/certbot
WORKDIR /var/www/html
ENTRYPOINT [ "certbot" ]
CMD [ "certonly", "--expand", "--noninteractive", "--webroot", "--webroot-path", "/var/www/certbot", "-d", "jorgebarreto.dev,www.jorgebarreto.dev,codedueler.jorgebarreto.dev,yasc.jorgebarreto.dev" ]