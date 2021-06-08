FROM ubuntu:20.04

ENV TZ=""
ENV DEBIAN_FRONTEND="noninteractive"

RUN apt update && apt install -y --no-install-recommends apache2 libapache2-mod-jk

# add the config files here

# volume

# expose
EXPOSE 80

CMD ["apachectl","-k","start","-DFOREGROUND"]