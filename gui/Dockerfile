FROM openjdk:8-jdk-alpine
VOLUME /tmp
ARG JAR_FILE

RUN apk update && apk add \
git 


COPY target/spring-openszzweb-2.1.0.BUILD-SNAPSHOT.jar  app.jar
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
