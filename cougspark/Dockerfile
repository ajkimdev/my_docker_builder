ARG BASE_CONTAINER=ajkimdev/basic-ubuntu
FROM $BASE_CONTAINER

ARG miniconda_version="4.8.3"
ARG miniconda_checksum="d63adf39f2c220950a063e0529d4ff74"
ARG conda_version="4.9.0"

ENV CONDA_DIR=/opt/conda \
    SHELL=/bin/bash \
    LC_ALL=en_US.UTF-8 \
    LANG=en_US.UTF-8 \
    LANGUAGE=en_US.UTF-8

ENV PATH=$CONDA_DIR/bin:$PATH \

ENV MINICONDA_VERSION="${miniconda_version}" \
    CONDA_VERSION="${conda_version}"