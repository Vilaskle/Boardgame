# # Use lightweight JDK base image
# FROM eclipse-temurin:17-jdk-alpine

# # Set working directory
# WORKDIR /app

# # Copy the JAR file from target folder into the image
# COPY target/database_service_project-0.0.2.jar app.jar

# # Command to run the JAR
# ENTRYPOINT ["java", "-jar", "app.jar"]


# Use a lightweight base image with JDK 17
FROM eclipse-temurin:17-jdk-alpine

# Set the working directory
WORKDIR /app

# Copy the JAR file (assuming only one .jar is in target/)
COPY target/*.jar app.jar

# Expose the default Spring Boot port (optional, but good practice)
EXPOSE 8080

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
