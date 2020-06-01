From ubuntu
RUN apt-get -y update --fix-missing
RUN apt-get install tzdata
RUN apt-get install -y apache2
RUN apt-get install -y apache2-utils
RUN apt-get install -y mysql-server
RUN apt-get install -y php libapache2-mod-php
COPY /Desktop/php-Dire/index.php /var/www/html/
WORKDIR /var/www/html/
Expose 80
CMD ["apache2ctl" , "-D" , "FOREGROUND"]
 
