# docker build -t hpc-centos:mpich-latest .

ARG base_image="os-base:centos-latest"
FROM "$base_image"

LABEL maintainer "An-Cheng Yang<acyang0903@gmail.com>"

RUN yum install -y mpich-3.2 mpich-3.2-devel mpich-3.2-autoload && yum clean all -y
