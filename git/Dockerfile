FROM alpine:3.8
MAINTAINER Cary Tan tx-cary@163.com
RUN echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/main" > /etc/apk/repositories
RUN echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/community" >> /etc/apk/repositories
RUN apk update && apk add vim && apk add git
VOLUME /workspace
WORKDIR /workspace
CMD /bin/sh
