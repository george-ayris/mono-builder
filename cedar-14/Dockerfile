FROM ubuntu:trusty
MAINTAINER ademar

RUN apt-get -q update
RUN apt-get -q -y install curl gcc g++ make wget unzip git autoconf pkg-config libtool automake build-essential mono-devel gettext

COPY build build
RUN chmod +x build
CMD ./build
