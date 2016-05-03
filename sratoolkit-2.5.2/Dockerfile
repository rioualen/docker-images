FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0


ENV SOURCE_DIR=~/app_sources
ENV BIN_DIR=~/bin

WORKDIR ${SOURCE_DIR}
RUN wget -nc http://ftp-trace.ncbi.nlm.nih.gov/sra/sdk/2.5.2/sratoolkit.2.5.2-ubuntu64.tar.gz
RUN tar xzf sratoolkit.2.5.2-ubuntu64.tar.gz
#RUN cp `find sratoolkit.2.5.2-ubuntu64/bin -maxdepth 1 -executable -type l` ${BIN_DIR}
#RUN ln -s -f ${SOURCE_DIR}/sratoolkit.2.5.2-ubuntu64/bin/fastq-dump ${BIN_DIR}/fastq-dump
#RUN cp -p ${SOURCE_DIR}/sratoolkit.2.5.2-ubuntu64/bin/fastq-dump /usr/local/bin


RUN ls -p ${SOURCE_DIR}
RUN ls -p ${SOURCE_DIR}/sratoolkit.2.5.2-ubuntu64
RUN ls -p ${SOURCE_DIR}/sratoolkit.2.5.2-ubuntu64/bin/

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
