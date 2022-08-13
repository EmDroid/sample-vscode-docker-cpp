FROM ubuntu:20.04
LABEL Description="Build environment"

RUN apt-get -qq update \
    && DEBIAN_FRONTEND=noninteractive apt-get -qq -y --no-install-recommends install \
        build-essential \
        ca-certificates \
        ccache \
        clangd \
        cmake \
        gdb \
        git \
        less \
        ninja-build \
        vim \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*
