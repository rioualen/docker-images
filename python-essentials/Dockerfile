FROM ubuntu:14.04
FROM rioualen/ubuntu-essentials:1.0

RUN apt-get update && apt-get -y install python-pip python-dev python3-pip python3.4-dev python-software-properties
RUN pip3 install numpy snakemake docutils pandas pyyaml && pip install numpy

ENTRYPOINT ["snakemake"]

MAINTAINER Claire Rioualen <claire.rioualen@inserm.fr>
