FROM "centos:latest"

RUN curl https://download-ib01.fedoraproject.org/pub/epel/7/x86_64/Packages/s/shc-4.0.3-1.el7.x86_64.rpm -o epel-release-shc.rpm
RUN rpm -Uvh epel-release*rpm
RUN yum -y install gcc

RUN mkdir /var/build

WORKDIR /var/build

ENTRYPOINT ["/usr/bin/shc"]