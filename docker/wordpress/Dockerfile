# Build a custom wordpress image with redis plugin
FROM wordpress:6-fpm-alpine

RUN apk --no-cache add autoconf g++ make \
  && pecl install redis-6.0.2 \
  && docker-php-ext-enable redis \
  && apk del autoconf g++ make;