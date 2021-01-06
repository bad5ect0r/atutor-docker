FROM php:5.5-apache
RUN a2enmod rewrite
RUN apt-get update && apt-get install -y libpng-dev libjpeg-dev
RUN docker-php-ext-configure gd --with-jpeg-dir
RUN docker-php-ext-install gd mysql mysqli
COPY ./atutor.conf /etc/apache2/sites-available/atutor.conf
RUN ln -s /etc/apache2/sites-available/atutor.conf /etc/apache2/sites-enabled/atutor.conf
COPY . /var/www/html/atutor
RUN mkdir /var/www/html/atutor/content
RUN mv /var/www/html/atutor/php.ini "$PHP_INI_DIR/php.ini"
RUN chown -R www-data: /var/www/html/atutor
