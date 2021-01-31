# docker build -t hpc-centos:openmpi-latest .

ARG base_image="os-base:centos-latest"
FROM "$base_image"

LABEL maintainer "An-Cheng Yang<acyang0903@gmail.com>"

RUN yum install -y openmpi3 openmpi3-devel && yum clean all -y

ENV PATH /usr/lib64/openmpi3/bin:$PATH

ENV LD_LIBRARY_PATH /usr/lib64/openmpi3/lib:$LD_LIBRARY_PATH
