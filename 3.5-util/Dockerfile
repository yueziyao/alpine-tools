FROM alpine:3.5

ENV LANG=C.UTF-8

RUN apk add --no-cache tzdata &&\
    cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime &&\
    echo "Asia/Shanghai" > /etc/timezone &&\
    apk del tzdata

RUN apk add --no-cache bash openssh openssh-sftp-server lftp rsync curl git
RUN ssh-keygen -A
RUN echo "root:root" | chpasswd &&\
    echo 'PermitRootLogin yes' >> /etc/ssh/sshd_config

EXPOSE 22
CMD ["/usr/sbin/sshd", "-D", "-e"]
