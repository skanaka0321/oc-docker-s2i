FROM redhat/ubi8

RUN yum update -y && \
  yum install -y httpd && \
  yum clean all
  
#RUN useradd -r -U -d /usr/local/apache2 -s /sbin/nologin apache
#RUN chown -R apache:apache /usr/local/apache2
USER apache

EXPOSE 80
CMD ["sudo", "httpd", "-DFOREGROUND"]
