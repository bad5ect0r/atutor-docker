FROM php:7.4-apache
RUN a2enmod rewrite
COPY ./atutor.conf /etc/apache2/sites-available/atutor.conf
RUN ln -s /etc/apache2/sites-available/atutor.conf /etc/apache2/sites-enabled/atutor.conf
COPY . /var/www/html/atutor
RUN mv /var/www/html/atutor/php.ini "$PHP_INI_DIR/php.ini"
RUN chown -R www-data: /var/www/html/atutor
