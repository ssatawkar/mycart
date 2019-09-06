#This is docker file for mycart MicroService frontend layer
# pull the image uf not exist
FROM centos:7
MAINTAINER author@gmail.com
RUN yum -y update 
RUN yum -y install httpd
ADD code /var/www/html
EXPOSE  80
ENV BACKENDLB=test
CMD ["apachectl", "-D", "FOREGROUND"]