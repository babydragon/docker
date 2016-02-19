FROM alpine
MAINTAINER jlj.babydragon@gmail.com
RUN apk add --no-cache git-svn=2.6.4-r0 git-perl=2.6.4-r0
RUN apk add --no-cache openssh-client

#RUN delgroup dialout && \
#	addgroup -g 20 staff &&  \
#	adduser -g 20 -u 501 -D babydragon

RUN mkdir /data
ADD id_rsa /root/.ssh/id_rsa

WORKDIR /data

ENTRYPOINT ["git"]
