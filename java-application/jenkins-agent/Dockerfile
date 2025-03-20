FROM maven:3.8.4-openjdk-17

RUN apt-get update && \
    apt-get install -y docker.io && \
    apt-get clean

WORKDIR /usr/src/app
