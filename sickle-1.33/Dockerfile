FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0


ENV SOURCE_DIR=~/app_sources/
ENV BIN_DIR=~/bin/


RUN cd ${SOURCE_DIR}
RUN wget https://github.com/najoshi/sickle/archive/v1.33.tar.gz
RUN tar xvfz v1.33.tar.gz
RUN cd sickle-1.33
RUN make
RUN cp sickle ${BIN_DIR}

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
