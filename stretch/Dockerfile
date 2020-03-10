FROM debian:stretch

RUN ln -sf /bin/bash /bin/sh

# Install required packages
RUN dpkg --add-architecture armhf
RUN apt-get update && \
	apt-get install -y \
	vim \
	ssh \
	unzip \
	bzip2 \
	wget \
	curl \
	rng-tools \
	crossbuild-essential-armhf \
	bc \
	liblz4-tool \
	debhelper \
	cpio \
	u-boot-tools \
	kmod \
	libc6-dev:armhf
