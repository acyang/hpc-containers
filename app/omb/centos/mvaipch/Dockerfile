# docker build -t centos-mvapich:omb-latest .

ARG base_image="acyang/hpc-centos:mvapich-latest"
FROM "$base_image"

LABEL maintainer "An-Cheng Yang<acyang0903@gmail.com>"

RUN cd /tmp && \
    wget http://mvapich.cse.ohio-state.edu/download/mvapich/osu-micro-benchmarks-5.7.tar.gz && \
    tar -zx -f osu-micro-benchmarks-5.7.tar.gz && \
    cd osu-micro-benchmarks-5.7 && \
    ./configure CC=$(which mpicc) CFLAGS=-O3 && \
    make -j2 && \
    make install && \
    cd .. && \
    rm -rf osu-micro-benchmarks-5.7*
