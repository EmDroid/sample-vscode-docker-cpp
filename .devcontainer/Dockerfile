FROM debian:bullseye
LABEL Description="Build environment"

RUN apt-get -qq update \
    && apt-get -qq -y --no-install-recommends install \
        build-essential \
        ca-certificates \
        gdb \
        git \
        less \
        vim \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*
