FROM ubuntu:16.04

MAINTAINER Rui Carmo https://github.com/rcarmo

RUN apt update \
 && apt dist-upgrade -y \
 && apt install -y \
     build-essential \
     libbz2-dev \
     libexpat1-dev \
     libffi-dev \
     libgdbm-dev \
     libjpeg-dev \
     liblapack-dev \
     libncurses5-dev \
     libreadline-dev \
     libssl-dev \
     libsqlite3-dev \
     libxml2-dev \
     libxslt-dev \
     lzma-dev \
     git \
     gfortran \
     wget \
     zlib1g-dev \
 && apt-get clean && rm -rf /var/lib/apt/lists/*

ARG VCS_REF
ARG VCS_URL
ARG BUILD_DATE
LABEL org.label-schema.vcs-ref=$VCS_REF \
      org.label-schema.vcs-url=$VCS_URL \
      org.label-schema.build-date=$BUILD_DATE