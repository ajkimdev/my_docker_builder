FROM adoptopenjdk/openjdk11:jdk-11.0.9_11.1-alpine
VOLUME /tmp
ARG JAR_FILE
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]