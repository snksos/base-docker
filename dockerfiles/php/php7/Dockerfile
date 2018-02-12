FROM phpdockerio/php7-fpm:latest

COPY ./sources.list.stretch /etc/apt/sources.list

RUN apt-get clean \
    && apt-get update \
    && apt-get -y --no-install-recommends install  php7.0-mysql php7.0-redis php7.0-gd \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*