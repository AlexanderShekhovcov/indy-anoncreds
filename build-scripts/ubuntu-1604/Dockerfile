FROM ubuntu:16.04

RUN apt-get update -y && apt-get install -y \
    # common stuff
        git \
        wget \
        unzip \
        python3.5 \
        python3-pip \
        python-setuptools \
        python3-venv \
    # fmp
        ruby \
        ruby-dev \
        rubygems \
        gcc \
        make \
    # pbc deps
        debhelper \
        autotools-dev \
        libreadline-dev \
        flex \
        bison \
        libtool \
        automake \
        libgmp-dev \
    # charm crypto
        openssl \
        libssl-dev

# install fpm
RUN gem install --no-ri --no-rdoc fpm

WORKDIR /root

ADD . /root
