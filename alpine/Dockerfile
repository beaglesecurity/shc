FROM "alpine:latest"

RUN echo "http://dl-cdn.alpinelinux.org/alpine/edge/testing" > /etc/apk/repositories \
  	&& echo "http://dl-cdn.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories \
  	&& echo "http://dl-cdn.alpinelinux.org/alpine/edge/main" >> /etc/apk/repositories

RUN apk update
RUN apk add gcc libc-dev bash shc

RUN mkdir /var/build

WORKDIR /var/build

ENTRYPOINT ["/bin/shc"]
