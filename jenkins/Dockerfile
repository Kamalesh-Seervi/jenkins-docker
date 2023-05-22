FROM ubuntu:latest
ARG DEBIAN_FRONTEND=noninteractive
WORKDIR /jenkins
RUN apt update
RUN apt upgrade -y
RUN apt install apache2 -y
RUN apt install php libapache2-mod-php  php-mysql -y
RUN apt install -y nano git 
COPY ./data/ .
RUN chmod +x /jenkins/main.sh 
CMD /jenkins/main.sh

