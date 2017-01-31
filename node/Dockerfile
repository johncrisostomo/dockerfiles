FROM resin/rpi-raspbian:latest
RUN apt-get update && \
	apt-get -qy install curl \
	build-essential python \
	ca-certificates xz-utils

WORKDIR /root/
RUN curl -O https://nodejs.org/dist/v7.4.0/node-v7.4.0-linux-armv7l.tar.xz
RUN tar -xJf node-*.tar.xz -C /usr/local --strip-components=1
CMD ["node"]
