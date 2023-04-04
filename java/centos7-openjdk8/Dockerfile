FROM registry.cn-chengdu.aliyuncs.com/jackiegu/centos7
MAINTAINER JackieGu<851469928@qq.com>
# LABEL author=JackieGu<851469928@qq.com>

ENV JAVA_PATH=/usr/local/java/openjdk/
ADD https://sso.jackiegu.cn/docker/java/openjdk/OpenJDK8U-jdk_x64_linux_hotspot_8u312b07.tar.gz $JAVA_PATH
RUN tar -xvf $JAVA_PATH/OpenJDK8U-jdk_x64_linux_hotspot_8u312b07.tar.gz -C $JAVA_PATH
RUN rm -f $JAVA_PATH/OpenJDK8U-jdk_x64_linux_hotspot_8u312b07.tar.gz

ENV JAVA_HOME=$JAVA_PATH/jdk8u312-b07/
ENV PATH=$PATH:$JAVA_HOME/bin

WORKDIR /usr/local
CMD /bin/bash
