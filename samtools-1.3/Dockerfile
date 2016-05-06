FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0

RUN apt-get update

ENV SOURCE_DIR=/root/app_sources/

WORKDIR ${SOURCE_DIR}
RUN wget --no-clobber http://sourceforge.net/projects/samtools/files/samtools/1.3/samtools-1.3.tar.bz2 && bunzip2 -f samtools-1.3.tar.bz2 && tar xvf samtools-1.3.tar
WORKDIR samtools-1.3
RUN make && make install

ENV PATH $PATH:/usr/local/bin

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
