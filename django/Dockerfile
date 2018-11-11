FROM python:3.7.1-alpine3.8
MAINTAINER Cary Tan tx-cary@163.com
ENV PS1='[django@docker $PWD]\$ '
RUN echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/main" > /etc/apk/repositories \
      && echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/community" >> /etc/apk/repositories \
      && apk update \
      && pip install Django -i https://mirrors.aliyun.com/pypi/simple/ \ 
      && mkdir -p /workspace
WORKDIR /workspace
CMD /bin/sh
