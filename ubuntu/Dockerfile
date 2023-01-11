# simple dockerfile to test OCP s2i using Dockerfile 

FROM centos:latest
MAINTAINER siva
RUN yum -y install httpd
COPY index.html /var/www/html/
CMD [“/usr/sbin/httpd”, “-D”, “FOREGROUND”]
EXPOSE 80

