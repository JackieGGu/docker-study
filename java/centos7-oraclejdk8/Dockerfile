FROM registry.cn-chengdu.aliyuncs.com/jackiegu/centos7
MAINTAINER JackieGu<851469928@qq.com>
# LABEL author=JackieGu<851469928@qq.com>

ENV JAVA_PATH=/usr/local/java/oraclejdk/
ADD https://sso.jackiegu.cn/docker/java/oraclejdk/jdk-8u311-linux-x64.tar.gz $JAVA_PATH
RUN tar -xvf $JAVA_PATH/jdk-8u311-linux-x64.tar.gz -C $JAVA_PATH
RUN rm -f $JAVA_PATH/jdk-8u311-linux-x64.tar.gz

ENV JAVA_HOME=$JAVA_PATH/jdk1.8.0_311/
ENV PATH=$PATH:$JAVA_HOME/bin

WORKDIR /usr/local
CMD /bin/bash
