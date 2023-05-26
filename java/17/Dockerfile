FROM ghcr.io/pterodactyl/yolks:java_17

USER root

RUN apt update && apt install wget
RUN wget -q -O /tmp/tinyspline.deb https://github.com/msteinbeck/tinyspline/releases/download/v0.6.0/tinyspline-0.6.0-Linux.deb \
    && dpkg -i /tmp/tinyspline.deb \
    && rm /tmp/tinyspline.deb

USER container