FROM php:7.0-fpm

# Install the PHP extensions we need for WordPress
# Extracted from original WordPress Dockerfile for PHP 7 FPM
RUN apt-get update && apt-get install -y libpng12-dev libjpeg-dev && rm -rf /var/lib/apt/lists/* \
	&& docker-php-ext-configure gd --with-png-dir=/usr --with-jpeg-dir=/usr \
	&& docker-php-ext-install gd mysqli
