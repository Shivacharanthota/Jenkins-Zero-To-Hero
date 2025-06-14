# Use Java 17 JDK base image
FROM eclipse-temurin:17-jdk-alpine

# Optional: Define artifact path
ARG artifact=target/spring-boot-web.jar

# Set work directory
WORKDIR /opt/app

# Copy app artifact
COPY ${artifact} app.jar

# Start application
# ENTRYPOINT ["java", "-jar", "app.jar"]
CMD ["tail", "-f", "/dev/null"]
