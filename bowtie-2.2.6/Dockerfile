FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0


ENV SOURCE_DIR=~/app_sources/
ENV BIN_DIR=~/bin/


WORKDIR ${SOURCE_DIR}

RUN wget --no-clobber http://downloads.sourceforge.net/project/bowtie-bio/bowtie2/2.2.6/bowtie2-2.2.6-linux-x86_64.zip;\
RUN unzip bowtie2-2.2.6-linux-x86_64.zip;\
RUN cp `find bowtie2-2.2.6/ -maxdepth 1 -executable -type f` ${BIN_DIR}
