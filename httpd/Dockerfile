FROM ubuntu:20.04

ENV TZ="America/New_York"
ENV DEBIAN_FRONTEND="noninteractive"

RUN apt update && apt install -y --no-install-recommends apache2 libapache2-mod-jk

# add the config files here
ADD apache2.conf /etc/apache2/apache2.conf
ADD 000-default.conf /etc/apache2/sites-enabled/000-default.conf
ADD worker.properties /etc/libapache2-mod-jk/workers.properties
ADD jk.conf /etc/apache2/mods-enabled/jk.conf

# volume
VOLUME ["/var/log/apache2"]

# expose
EXPOSE 80 443

CMD ["apachectl","-k","start","-DFOREGROUND"]