FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0
FROM rioualen/python-essentials:1.0
FROM bioconductor/release_core:latest

#RUN echo "deb http://cran.univ-lyon1.fr/bin/linux/ubuntu/trusty/" >> /etc/apt/sources.list
RUN apt-get update && apt-get -y install r-base r-base-dev libcurl4-openssl-dev libxml2-dev
RUN echo "r <- getOption('repos'); r['CRAN'] <- 'http://cran.us.r-project.org'; options(repos = r);" >> ~/.Rprofile

RUN Rscript -e "install.packages(c('XML', 'bPeaks', 'caTools'))" && Rscript -e "source('http://bioconductor.org/biocLite.R'); biocLite(c('affy', 'biomaRt', 'Rsamtools'))"

RUN apt-get -y install python3-pip && pip3 install "rpy2<2.5.6" ## to be removed !

ENTRYPOINT ["R"]

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
