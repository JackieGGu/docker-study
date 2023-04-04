FROM registry.cn-chengdu.aliyuncs.com/jackiegu/centos7
MAINTAINER JackieGu<851469928@qq.com>
# LABEL author=JackieGu<851469928@qq.com>

ENV JAVA_PATH=/usr/local/java/openjdk/
ADD https://sso.jackiegu.cn/docker/java/openjdk/openjdk-11.0.2_linux-x64_bin.tar.gz $JAVA_PATH
RUN tar -xvf $JAVA_PATH/openjdk-11.0.2_linux-x64_bin.tar.gz -C $JAVA_PATH
RUN rm -f $JAVA_PATH/openjdk-11.0.2_linux-x64_bin.tar.gz

ENV JAVA_HOME=$JAVA_PATH/jdk-11.0.2/
ENV PATH=$PATH:$JAVA_HOME/bin

WORKDIR /usr/local
CMD /bin/bash
