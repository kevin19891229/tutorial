FROM  centos:7
MAINTAINER yb19891229

USER root

ENV OPT_DIR /opt

RUN yum -y install gcc

RUN mkdir $OPT_DIR/test
COPY ./src/main.c $OPT_DIR/test

RUN gcc $OPT_DIR/test/main.c -o $OPT_DIR/test/main

ENTRYPOINT ["/opt/test/main"]
