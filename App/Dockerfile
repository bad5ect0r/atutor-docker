FROM php:7.3-apache
RUN apt-get update && apt-get install -y php7-gd 
RUN a2enmod rewrite
COPY ./atutor.conf /etc/apache2/sites-available/atutor.conf
RUN ln -s /etc/apache2/sites-available/atutor.conf /etc/apache2/sites-enabled/atutor.conf
COPY . /var/www/html/atutor
RUN chown -R www-data: /var/www/html/atutor
