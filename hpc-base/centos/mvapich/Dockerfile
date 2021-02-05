# docker build -t hpc-centos:mvapich-latest .

ARG base_image="acyang/os-base:centos-latest"
FROM "$base_image"

LABEL maintainer "An-Cheng Yang<acyang0903@gmail.com>"

RUN yum install -y mvapich23 mvapich23-devel && yum clean all -y

ENV PATH /usr/lib64/mvapich23/bin:$PATH

ENV LD_LIBRARY_PATH /usr/lib64/mvapich23/lib:$LD_LIBRARY_PATH
