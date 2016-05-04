FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0


ENV SOURCE_DIR=/root/app_sources/
ENV BIN_DIR=/root/bin/


WORKDIR ${SOURCE_DIR}
RUN wget --no-clobber http://downloads.sourceforge.net/project/bowtie-bio/bowtie/1.1.1/bowtie-1.1.1-linux-x86_64.zip && unzip bowtie-1.1.1-linux-x86_64.zip

WORKDIR ${BIN_DIR}
RUN cp `find ${SOURCE_DIR}bowtie-1.1.1/ -maxdepth 1 -executable -type f` .

ENV PATH $PATH:/usr/local/bin


MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
