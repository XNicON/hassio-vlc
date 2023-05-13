ARG BUILD_FROM=hassioaddons/base:14.0.0

FROM $BUILD_FROM AS build-base

ENV LANG C.UTF-8
ENV HOME=/home/vlc

RUN apk update
RUN apk add --no-cache alsa-plugins-pulse
RUN apk add --no-cache vlc

RUN sed -i 's/geteuid/getppid/' /usr/bin/vlc
RUN sed -i '197s#.*#    dir = dir == undefined ? "file:///media" : dir;#' /usr/share/vlc/lua/http/js/controllers.js

ENTRYPOINT [ "/init" ]
CMD []
COPY root /
