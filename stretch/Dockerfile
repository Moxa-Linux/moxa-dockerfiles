FROM debian:stretch

# Moxa APT source
RUN echo "deb http://debian.moxa.com/debian stretch main contrib non-free" > /etc/apt/sources.list.d/moxa.sources.list

RUN dpkg --add-architecture armhf
RUN apt-get update -qqy && apt-get install -qqy apt-utils dialog

# Moxa archive keyring
RUN apt-get install -qqy --allow-unauthenticated moxa-archive-keyring

# General tools
RUN apt-get install -qqy curl wget gzip bzip2 vim git

# Debian package
RUN apt-get install -qqy devscripts

# GNU
RUN apt-get install -qqy libtool bc

# Kernel
RUN apt-get install -qqy libncurses5-dev liblz4-tool u-boot-tools device-tree-compiler initramfs-tools kmod

# Build
RUN apt-get install -qqy crossbuild-essential-armhf pkg-config:armhf
