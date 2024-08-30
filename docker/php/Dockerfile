FROM php:8.3-fpm-alpine
#composerインストール
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer
#拡張パッケージインストール
RUN apk update
RUN apk add git
#php拡張機能インストール
RUN docker-php-ext-install pdo pdo_mysql