# Docker image for springboot file run
# VERSION 0.0.1
# Author: eangulee
# 基础镜像使用java
FROM openjdk:11.0.8-jdk
# 作者
MAINTAINER zuoyao <zuoyao@xosw.com>
VOLUME ["/opt/software/logs/eureka-server"]
# 将jar包添加到容器中并更名为app.jar
ADD eureka-server-1.0.1.jar app.jar
# 运行jar包
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]

# PORT
EXPOSE 8761
