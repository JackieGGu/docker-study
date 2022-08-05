FROM centos:7
MAINTAINER JackieGu<851469928@qq.com>
# LABEL author=JackieGu<851469928@qq.com>

RUN yum -y install net-tools
RUN yum -y install vim
RUN yum -y install less

COPY timezone/Shanghai /etc/localtime
RUN echo 'Asia/Shanghai' > /etc/timezone

WORKDIR /usr/local
CMD /bin/bash
