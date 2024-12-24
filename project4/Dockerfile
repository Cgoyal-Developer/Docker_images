FROM ubuntu:latest
LABEL "Project"="Pankaj Sharma"
ENV DEBIAN_FRONTEND=noninteractive


RUN apt update && apt install git -y
RUN apt install apache2 -y

WORKDIR /var/www/html/
ADD  2136_kool_form_pack.tar.gz /var/www/html/
CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"]
VOLUME /var/log/apache2
EXPOSE 80
