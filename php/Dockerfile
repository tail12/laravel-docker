FROM php:7.2.12-fpm

RUN apt-get update \
    && apt-get install -y zlib1g-dev libpq-dev iputils-ping net-tools git

RUN git clone https://github.com/phpredis/phpredis.git /usr/src/php/ext/redis
RUN docker-php-ext-install pdo_pgsql pgsql mbstring
