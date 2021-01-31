# docker build -t os-base:centos-latest .

FROM centos:centos7.9.2009

LABEL maintainer "An-Cheng Yang<acyang0903@gmail.com>"

ENV LANG=C.UTF-8 LC_ALL=C.UTF-8 TZ=Asia/Taipei

RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN yum install -y gcc gcc-c++ gcc-gfortran make which wget pkgconfig cmake bzip2&& yum clean all -y


