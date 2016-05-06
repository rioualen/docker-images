FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0


ENV SOURCE_DIR=/root/app_sources
ENV BIN_DIR=/root/bin

WORKDIR ${SOURCE_DIR}
RUN wget -nc http://ftp-trace.ncbi.nlm.nih.gov/sra/sdk/2.5.2/sratoolkit.2.5.2-ubuntu64.tar.gz && tar xzf sratoolkit.2.5.2-ubuntu64.tar.gz

WORKDIR ${BIN_DIR}
RUN ln -s -f ${SOURCE_DIR}/sratoolkit.2.5.2-ubuntu64/bin/fastq-dump .

ENV PATH $PATH:/root/bin

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
