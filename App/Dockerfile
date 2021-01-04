FROM ubuntu:16.04
RUN apt-get update
RUN apt-get install -y apache2 libapache2-mod-php
RUN systemctl start apache2
RUN apt-get install php5 libapache2-mod-php5 php5-mcrypt php5-mysql php5-gd
# COPY . /var/www/html/atutor
# RUN chown -R www-data: /var/www/html/atutor/
# RUN a2enmod rewrite
# RUN touch /etc/apache2/sites-available/atutor.conf
# RUN ls -s /etc/apache2/sites-available/atutor.conf /etc/apache2/sites-enabled/atutor.conf

