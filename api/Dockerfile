FROM php:7.4-apache 

RUN apt-get update

RUN apt-get install -y libzip-dev libjpeg62-turbo-dev libpng-dev libfreetype6-dev

# Install extensions

#RUN docker-php-ext-install pdo_mysql mbstring zip exif pcntl
RUN docker-php-ext-install pdo_mysql zip exif pcntl

#RUN docker-php-ext-configure gd –-with-gd –-with-freetype-dir=/usr/include/ –-with-jpeg-dir=/usr/include/ –-with-png-dir=/usr/include/
RUN docker-php-ext-configure gd --with-freetype --with-jpeg

RUN docker-php-ext-install gd