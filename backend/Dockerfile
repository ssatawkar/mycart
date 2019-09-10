#This is docker file for mycart MicroService frontend layer
# pull the image uf not exist
FROM centos:7
MAINTAINER author@gmail.com
RUN yum -y update 
RUN yum -y install httpd php php-gd php-mysql
ADD code /var/www/html
EXPOSE  80
ENV MY_DB_HOST_WRITE=test MY_DB_NAME=test MY_DB_USER=test MY_DB_PASS=test MY_DB_HOST_READ=test
CMD ["apachectl", "-D", "FOREGROUND"]