FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0


ENV SOURCE_DIR=~/app_sources/
ENV BIN_DIR=~/bin/

#RUN apt-get -y install unzip

WORKDIR ${SOURCE_DIR}
RUN wget --no-clobber http://www.bioinformatics.babraham.ac.uk/projects/fastqc/fastqc_v0.11.5.zip
RUN unzip -o fastqc_v0.11.5.zip
RUN chmod +x FastQC/fastqc
RUN ln -s -f ${SOURCE_DIR}/FastQC/fastqc ${BIN_DIR}/fastqc

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
