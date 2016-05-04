FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0


ENV SOURCE_DIR=/root/app_sources/
ENV BIN_DIR=/root/bin/


WORKDIR ${SOURCE_DIR}
WORKDIR homer
RUN wget "http://homer.salk.edu/homer/configureHomer.pl" && perl configureHomer.pl -install homer

WORKDIR ${BIN_DIR}
RUN cp `find ${SOURCE_DIR}homer/bin -maxdepth 1 -executable -type f` .

ENV PATH $PATH:/root/bin


MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>


