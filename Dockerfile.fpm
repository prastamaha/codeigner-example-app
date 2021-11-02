# source image 
FROM php:7.4-fpm

# install app dependencies
RUN apt-get update && \
    apt-get install -y curl \
    build-essential \
    libssl-dev \
    zlib1g-dev \
    libpng-dev \
    libjpeg-dev \
    libfreetype6-dev \
    libicu-dev 

# install mysql driver
RUN docker-php-ext-install mysqli pdo_mysql

COPY . /var/www
WORKDIR /var/www

RUN apt-get clean && rm -rf /var/lib/apt/lists/*

EXPOSE 9000
CMD ["php-fpm"]
