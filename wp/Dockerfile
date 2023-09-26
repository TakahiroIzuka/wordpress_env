FROM wordpress:php7.4

ENV PHP_IDE_CONFIG="serverName=wp"

# パッケージのインストール
# RUN pecl install xdebug && docker-php-ext-enable xdebug
RUN apt-get update && apt-get install -y \
    git \
    vim \
    sudo \
    locales-all

ENV LANG ja_JP.UTF-8
ENV LANGUAGE ja_JP:ja
ENV LC_ALL ja_JP.UTF-8

RUN "/bin/bash"

COPY ./wp/xdebug.ini /usr/local/etc/php/conf.d/