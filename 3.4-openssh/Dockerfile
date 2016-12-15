FROM helphi/alpine:3.4

MAINTAINER helphi

RUN apk add --no-cache openssh openssh-sftp-server &&\
    ssh-keygen -A

CMD ["/usr/sbin/sshd", "-D", "-e"]
