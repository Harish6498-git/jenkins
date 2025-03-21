# Use a base image that includes Maven and Java 11 (Alpine-based)
FROM maven:3.8.6-openjdk-11-slim

# Install Docker CLI (Alpine-specific)
RUN apk update && apk add --no-cache docker-cli

# Set the working directory
WORKDIR /app

# Copy the application JAR (Assuming it's built in the 'target' directory)
COPY target/spring-boot-web.jar app.jar

# Expose the port your application listens on (if applicable)
# EXPOSE 8080

# Define the command to run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
