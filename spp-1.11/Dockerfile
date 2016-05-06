FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0
FROM rioualen/r-essentials:1.0

ENV SOURCE_DIR=/root/app_sources/
ENV BIN_DIR=/root/bin/

RUN apt-get -y install libboost-dev             # should be removable

WORKDIR ${SOURCE_DIR}
RUN wget http://compbio.med.harvard.edu/Supplements/ChIP-seq/spp_1.11.tar.gz
RUN R CMD INSTALL spp_1.11.tar.gz


MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
