FROM helphi/alpine:3.4

MAINTAINER helphi

RUN apk add --no-cache openssh &&\
    ssh-keygen -A

CMD ["/usr/sbin/sshd", "-D", "-e"]