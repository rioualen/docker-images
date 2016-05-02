FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0
FROM rioualen/R-essentials:1.0

ENV SOURCE_DIR=~/app_sources/
ENV BIN_DIR=~/bin/


RUN cd ${SOURCE_DIR}
RUN wget http://compbio.med.harvard.edu/Supplements/ChIP-seq/spp_1.11.tar.gz
RUN sudo R CMD INSTALL spp_1.11.tar.gz


MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
