FROM ubuntu:16.04
LABEL maintainer="niceman114@gmail.com"

RUN echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | debconf-set-selections && \
    apt-get update && \
    apt-get install -y --no-install-recommends software-properties-common && \
    add-apt-repository ppa:webupd8team/java && \
    apt-get update && \
    apt-get install -y --no-install-recommends oracle-java8-installer && \
    rm -rf /var/lib/apt/lists/*