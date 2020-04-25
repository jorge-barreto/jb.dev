FROM nginx:1.16.1-alpine

COPY ./nginx_conf /etc/nginx/
COPY ./nginx_webroot /usr/share/nginx/html/

RUN rm -f /var/log/nginx/access.log \
	&& rm -f /var/log/nginx/error.log \
  && touch /var/log/nginx/access.log \
  && touch /var/log/nginx/error.log
