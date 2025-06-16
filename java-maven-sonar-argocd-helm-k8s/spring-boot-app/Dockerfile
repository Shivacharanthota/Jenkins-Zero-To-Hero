# Use Java 17 JDK base image
FROM eclipse-temurin:17-jdk-alpine

RUN apk update && \
    apk add --no-cache maven git docker-cli

WORKDIR /opt/app

# Copy the built JAR regardless of version
COPY target/*.jar app.jar

CMD ["java", "-jar", "app.jar"]
