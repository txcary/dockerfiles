FROM alpine:3.8
MAINTAINER Cary Tan tx-cary@163.com
ENV PS1='[truffle@docker $PWD]\$ '
RUN echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/main" > /etc/apk/repositories \
      && echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/community" >> /etc/apk/repositories \
      && apk update \
      && apk add npm \
      && mkdir -p /workspace \
      && npm config set registry https://registry.npm.taobao.org \
      && npm install -g truffle
WORKDIR /workspace
CMD /bin/sh
