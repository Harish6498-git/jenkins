# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM openjdk:17-alpine


# Install Docker using apk (Alpine's package manager)
RUN apk update && \
    apk add --no-cache docker

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

 COPY target/spring-boot-web.jar app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]