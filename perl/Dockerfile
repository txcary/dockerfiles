FROM alpine:3.8
MAINTAINER Cary Tan tx-cary@163.com
ENV PS1='[perl@docker $PWD]\$ '
ENV LC_ALL='en_US.UTF-8'
ENV LANG='en_US.UTF-8'
RUN echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/main" > /etc/apk/repositories \
      && echo "http://mirrors.tuna.tsinghua.edu.cn/alpine/v3.8/community" >> /etc/apk/repositories \
      && apk update \
      && apk add perl perl-lwp-useragent-determined perl-xml-simple perl-html-tree perl-spreadsheet-parseexcel perl-json \
      && mkdir -p /workspace
WORKDIR /workspace
CMD /bin/sh
