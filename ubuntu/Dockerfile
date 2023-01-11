# simple dockerfile to test OCP s2i using Dockerfile 

#FROM ubuntu:18.04
#CMD ["/bin/bash", "-c", "sleep infinity"]
#FROM httpd:2.4
#CMD ["/bin/bash", "-c", "--", "while true; do sleep 7200; done;"]

FROM ubuntu
RUN apt update 
RUN apt install –y apache2 
RUN apt install –y apache2-utils 
RUN apt clean 
EXPOSE 80
CMD [“apache2ctl”, “-D”, “FOREGROUND”]


