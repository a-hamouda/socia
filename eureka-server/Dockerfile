FROM openjdk:17-slim
RUN apt-get -y update; apt-get -y install curl
EXPOSE 8761
ARG JAR_FILE=target/*.jar
ADD ${JAR_FILE} app.jar
ENTRYPOINT ["java", "-jar", "/app.jar"]
