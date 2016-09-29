FROM alpine:3.4

MAINTAINER helphi

ENV LANG=C.UTF-8

RUN apk add --no-cache tzdata &&\
    cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime &&\
    echo "Asia/Shanghai" > /etc/timezone &&\
    apk del tzdata