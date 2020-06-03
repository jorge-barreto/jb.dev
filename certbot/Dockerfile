FROM certbot/certbot
WORKDIR /var/www/html
ENTRYPOINT [ "certbot" ]
CMD [ "certonly", "--expand", "--noninteractive", "--webroot", "--webroot-path", "/www", "-d", "jorgebarreto.dev,www.jorgebarreto.dev,codedueler.jorgebarreto.dev,cdj.jorgebarreto.dev,yasc.jorgebarreto.dev,larv.jorgebarreto.dev" ]