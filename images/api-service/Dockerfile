FROM tutum/apache-php
MAINTAINER Teerasak Vichadee <teerasak_vic@ascendinter.com>

RUN    apt-get update \
    && apt-get install -yq git \
    && rm -rf /var/lib/apt/lists/*

# Clear application folder
RUN rm -fr /app
# ADD . /app

# Install composer
# RUN composer install
