FROM nginx:alpine
RUN set -x ; \
  addgroup -g 82 -S www-data ; \
  adduser -u 82 -D -S -G www-data www-data && exit 0 ; exit 1
COPY ./ /etc/nginx/
RUN ln -s /var/log/nginx /etc/nginx/logs
