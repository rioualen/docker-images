FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0


ENV SOURCE_DIR=~/app_sources/

WORKDIR ${SOURCE_DIR}
RUN wget --no-clobber https://github.com/arq5x/bedtools2/releases/download/v2.24.0/bedtools-2.24.0.tar.gz
RUN tar xvfz bedtools-2.24.0.tar.gz
WORKDIR bedtools2
RUN make
RUN make install

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
