FROM        progrium/busybox 
MAINTAINER  Ross Merrigan <email@rossmerrigan.com>

RUN opkg-install curl ca-certificates

ENV MONO_HOME /usr/mono

RUN curl "http://github.com/mono/mono/archive/mono-4.0.2.5.tar.gz" 

RUN ./autogen.sh --prefix=$MONO_HOME

RUN MAKE

RUN MAKE INSTALL