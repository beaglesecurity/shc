FROM "ubuntu:focal"

RUN apt-get update
RUN apt-get install -y software-properties-common
RUN add-apt-repository ppa:neurobin/ppa
RUN apt-get update
RUN apt-get install -y shc gcc gcc-aarch64-linux-gnu

RUN mkdir /var/build

WORKDIR /var/build

ENTRYPOINT ["/usr/bin/shc"]
