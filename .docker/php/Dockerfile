FROM php:8.2-fpm-alpine

COPY php.ini /usr/local/etc/php

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

RUN apk update \
    && apk add -U --no-cache \
        git \
        zip \
        unzip
