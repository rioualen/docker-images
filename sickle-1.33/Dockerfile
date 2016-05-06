FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0


ENV SOURCE_DIR=/root/app_sources/
ENV BIN_DIR=/root/bin/


WORKDIR ${SOURCE_DIR}
RUN wget https://github.com/najoshi/sickle/archive/v1.33.tar.gz && tar xvfz v1.33.tar.gz
WORKDIR sickle-1.33
RUN make
WORKDIR ${BIN_DIR}
RUN cp ${SOURCE_DIR}sickle-1.33/sickle .

ENV PATH $PATH:/root/bin


MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
