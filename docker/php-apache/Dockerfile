# source image 
FROM php:7.4-apache

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

# enable apache module
RUN a2enmod rewrite headers

# copy app to apache root directory
COPY . /var/www/html
