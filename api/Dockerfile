FROM php:7.3.6-fpm-alpine3.9
RUN apk add --no-cache openssl bash mysql-client nodejs npm alpine-sdk
RUN docker-php-ext-install pdo pdo_mysql

WORKDIR /var/www

RUN rm -rf /var/www/html
RUN ln -s public html

RUN php -r "readfile('http://getcomposer.org/installer');" | php -- --install-dir=/usr/bin/ --filename=composer

EXPOSE 9000