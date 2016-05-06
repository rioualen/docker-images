FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0


ENV SOURCE_DIR=/root/app_sources/
ENV BIN_DIR=/root/bin/

#RUN apt-get -y install unzip                ## to be removed !!

WORKDIR ${SOURCE_DIR}
RUN wget --no-clobber http://www.bioinformatics.babraham.ac.uk/projects/fastqc/fastqc_v0.11.5.zip && unzip -o fastqc_v0.11.5.zip && chmod +x FastQC/fastqc
WORKDIR ${BIN_DIR}
RUN ln -s ${SOURCE_DIR}FastQC/fastqc .

ENV PATH $PATH:/root/bin

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
