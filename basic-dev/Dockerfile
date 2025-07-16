FROM ubuntu:24.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update && \
    apt install -y \
    fish \
    git \
    build-essential \
    gdb \
    clang \
    cmake \
    lldb \
    libssl-dev \
    pkg-config \
    curl \
    ca-certificates \
    python3-setuptools \
    protobuf-compiler \
    libprotobuf-dev \
    && rm -rf /var/lib/apt/lists/*

RUN chsh -s /usr/bin/fish root

CMD ["tail", "-f", "/dev/null"]
