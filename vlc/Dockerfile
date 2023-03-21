FROM hassioaddons/base:13.1

ENV LANG C.UTF-8
ENV HOME=/home/vlc

RUN apk update
RUN apk add --no-cache alsa-plugins-pulse
RUN apk add --no-cache vlc

ENTRYPOINT [ "/init" ]
CMD []
COPY root /
