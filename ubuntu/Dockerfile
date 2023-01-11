FROM redhat/ubi8

RUN yum update -y && \
  yum install -y httpd && \
  yum clean all

EXPOSE 80

USER root
CMD ["sudo", "httpd", "-DFOREGROUND"]
