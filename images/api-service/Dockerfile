FROM php:5.6-apache
MAINTAINER Teerasak Vichadee <teerasak_vic@ascendinter.com>

# Install required modules
RUN apt-get update && apt-get install -y \
    libfreetype6-dev \
    libjpeg62-turbo-dev \
    libmcrypt-dev \
    libpng12-dev \
    && docker-php-ext-install iconv mcrypt \
    && docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ \
    && docker-php-ext-install gd \
    && docker-php-ext-install pdo \
    && docker-php-ext-install mbstring \
    && docker-php-ext-install tokenizer

# CMD ["php"]
