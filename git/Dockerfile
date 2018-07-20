FROM alpine:3.8
MAINTAINER Cary Tan tx-cary@163.com
ENV PS1='[git@docker $PWD]\$ '
RUN echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/main" > /etc/apk/repositories \
      && echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/community" >> /etc/apk/repositories \
      && apk update \
      && apk add git git-doc \
      && mkdir -p /workspace
WORKDIR /workspace
CMD /bin/sh
