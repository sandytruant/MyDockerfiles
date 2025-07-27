FROM ubuntu:24.04

RUN apt update && DEBIAN_FRONTEND=noninteractive apt install -y sudo \
    && rm -rf /var/lib/apt/lists/*

RUN useradd -m -s /bin/bash -G sudo abc

RUN echo "abc:password" | chpasswd

RUN echo "abc ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers

USER abc

WORKDIR /home/abc

CMD ["bash"]