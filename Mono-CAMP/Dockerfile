FROM ubuntu:latest
# add timezone conf
ENV TZ=Asia/Kolkata
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN apt-get update
RUN apt-get install php mariadb-server apache2 -y

#RUN service apache2 restart

EXPOSE 80 3306

#ENTRYPOINT /bin/bash
ENTRYPOINT ["tail", "-f", "/dev/null"]
