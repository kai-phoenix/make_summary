FROM php:8.3-fpm
#依存関係のインストール
RUN apt-get update && apt-get install -y \
    libzip-dev \
    zip \
    unzip \
    mbstring \
    exif \
    && docker-php-ext-install pdo_mysql

#composerのインストール
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
