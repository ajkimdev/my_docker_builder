ARG ROOT_CONTAINER=ubuntu:focal@sha256:1d7b639619bdca2d008eca2d5293e3c43ff84cbee597ff76de3b7a7de3e84956

ARG BASE_CONTAINER=$ROOT_CONTAINER
FROM $BASE_CONTAINER

USER root
ENV HOME=/root
WORKDIR $HOME

RUN apt update \
    && apt install -yq --no-install-recommends \
    wget \
    bzip2 \
    ca-certificates \
    locales \
    fonts-liberation \
    vim \
    git \
    zsh \
    net-tools \
    openssh-server \
    openssh-client \
    && apt clean

RUN echo "en_US.UTF-8 UTF-8" > /etc/locale.gen && \
    locale-gen

RUN sh -c "$(wget -O- https://github.com/deluan/zsh-in-docker/releases/download/v1.1.1/zsh-in-docker.sh)" -- \
    -t agnoster

RUN echo "if [ -t 1 ]; then" >> /root/.bashrc
RUN echo "exec zsh" >> /root/.bashrc
RUN echo "fi" >> /root/.bashrc