FROM erzhu4/php72-nginx:latest as php-env

RUN apt-get update && apt-get install -y \
	php7.2-zip \
	php-mbstring \
	php-xml \
	php7.2-fpm \
	composer \
	nodejs \
	npm \
	libpng-dev \
	redis \
	php7.2-sqlite \
	supervisor \
	&& composer global require "laravel/installer"

RUN echo "daemon off;" >> /etc/nginx/nginx.conf

CMD service php7.2-fpm start && nginx

RUN echo "laravel with php7.2 and nginx docker file"