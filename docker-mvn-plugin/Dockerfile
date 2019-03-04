#pull java image
FROM openjdk:8-jdk-alpine

LABEL maintainer="Siva Nagi Reddy Alla <siva.alla@outlook.com>"

VOLUME /tmp
ARG JAR_FILE
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]