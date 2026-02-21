FROM emscripten/emsdk:5.0.0

RUN ln -fs /usr/share/zoneinfo/America/New_York /etc/localtime \
    && DEBIAN_FRONTEND="noninteractive" apt-get update && apt-get -y install tzdata \
    && dpkg-reconfigure --frontend noninteractive tzdata

RUN curl -fsSL https://apt.kitware.com/kitware-archive.sh | sh

RUN apt-get update \
    && apt-get install -y \
        build-essential \
        gcc \
        g++ \
        gdb \
        clang \
        cmake \
        make \
        ninja-build \
        cmake \
        autoconf \
        automake \
        libtool \
        valgrind \
        locales-all \
        dos2unix \
        rsync \
        tar \
    && apt-get clean
