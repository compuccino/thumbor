# Ubuntu xenial 16.04 base image
FROM ubuntu:16.04

# update package lists
RUN apt-get update

# upgrade installed packages
RUN apt-get upgrade --yes

# install circle ci dependencies
RUN apt-get --yes install git ssh tar gzip ca-certificates

# install thumbor dependencies
RUN apt-get --yes install python
RUN apt-get --yes install python-setuptools
RUN apt-get --yes install gcc
RUN apt-get --yes install libssl-dev
RUN apt-get --yes install libcurl4-openssl-dev
RUN apt-get --yes install python-numpy
RUN apt-get --yes install python-opencv
RUN apt-get --yes install libopencv-dev
RUN apt-get --yes install libjpeg-dev
RUN apt-get --yes install libpng-dev
RUN apt-get --yes install libx264-dev
RUN apt-get --yes install libass-dev
RUN apt-get --yes install libvpx-dev
RUN apt-get --yes install libwebp-dev
RUN apt-get --yes install webp
RUN apt-get --yes install gifsicle
RUN apt-get --yes install memcached
RUN apt-get --yes install libmemcache-dev
RUN apt-get --yes install libmemcached-dev
RUN apt-get --yes install python-pyexiv2
RUN apt-get --yes install cython

# set circle ci non-root user
RUN useradd -ms /bin/bash circleci
USER circleci
WORKDIR /home/circleci
