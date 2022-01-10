#Pulling ubuntu docker image
FROM ubuntu

MAINTAINER macan_ubuntu

ARG DEBIAN_FRONTEND=noninteractive

#Update and Upgrade the ubuntu system
RUN apt update; apt dist=upgrade -y

#Installing apache as webserver and mariadb-server as database server
RUN apt install -y apache2 mariadb-server

#Running entrypoint for apache
ENTRYPOINT apachectl -D FOREGROUND

