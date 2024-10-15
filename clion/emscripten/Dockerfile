FROM emscripten/emsdk

RUN ln -fs /usr/share/zoneinfo/America/New_York /etc/localtime \
    && DEBIAN_FRONTEND="noninteractive" apt-get update && apt-get -y install tzdata \
    && dpkg-reconfigure --frontend noninteractive tzdata

RUN apt-get update \
    && apt-get install -y \
        build-essential \
        gcc \
        g++ \
        gdb \
        clang \
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
