FROM redhat/ubi8

RUN yum update -y && \
  yum install -y httpd && \
  yum clean all
  
USER apache

RUN useradd -r -U -d /usr/local/apache2 -s /sbin/nologin apache
RUN chown -R apache:apache /usr/local/apache2


EXPOSE 8080
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
