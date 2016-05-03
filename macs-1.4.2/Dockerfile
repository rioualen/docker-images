FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0

RUN cd ${SOURCE_DIR}

RUN wget --no-clobber https://github.com/downloads/taoliu/MACS/MACS-1.4.2-1.tar.gz
RUN tar xvfz MACS-1.4.2-1.tar.gz
WORKDIR MACS-1.4.2
RUN python setup.py install

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
