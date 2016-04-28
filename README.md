# docker-firefox-webatm

*container 環境配置*
$ xhost +
$ docker run --rm -it -e DISPLAY=unix$DISPLAY \
   -v /tmp/.X11-unix:/tmp/.X11-unix 32bit/ubuntu:14.04 bash

*firefox in docker*
$ xhost +
$ docker run --privileged --rm -it -e DISPLAY=unix$DISPLAY \
   -v /tmp/.X11-unix:/tmp/.X11-unix -v /dev/bus/usb:/dev/bus/usb \
   -v /tmp:/mnt ubuntu1404:i386 bash
# pcscd
# firefox
