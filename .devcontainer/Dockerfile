FROM debian:bullseye
LABEL Description="Build environment"

RUN apt-get -qq update \
    && apt-get -qq -y --no-install-recommends install \
        build-essential \
        ca-certificates \
        clangd \
        cmake \
        gdb \
        git \
        less \
        ninja-build \
        vim \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*
