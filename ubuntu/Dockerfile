FROM rhel7:7.5
LABEL description="This is a custom httpd container image"
RUN yum install -y httpd
EXPOSE 80
ENV LogLevel "info"
USER apache
ENTRYPOINT ["/usr/sbin/httpd"]
CMD ["-D", "FOREGROUND"]
