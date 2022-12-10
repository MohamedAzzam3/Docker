FROM ubuntu
RUN apt update 
RUN apt install apache2 -y
RUN apt install apache2-utils -y
RUN apt clean
COPY ./hello-world.html /var/www/html
COPY ./httpd.conf /usr/local/apache2/conf/httpd.conf
ENV CONTAINER=docker
EXPOSE 9999
CMD ["apache2ctl","-D","FOREGROUND"]
