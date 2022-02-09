FROM ubuntu:20.04

LABEL maintainer="imalyshok@gmail.com"
ENV TZ=Europe/Kiev
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN apt-get update
RUN apt-get install apache2 -y
RUN apt-get install apache2-utils -y
RUN apt install net-tools -y
RUN apt install curl -y
RUN apt-get clean
EXPOSE 80
CMD  [ "/usr/sbin/apache2ctl", "-D", "FOREGROUND"]