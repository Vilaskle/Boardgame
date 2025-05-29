# # Use lightweight JDK base image
# FROM eclipse-temurin:17-jdk-alpine

# # Set working directory
# WORKDIR /app

# # Copy the JAR file from target folder into the image
# COPY target/database_service_project-0.0.2.jar app.jar

# # Command to run the JAR
# ENTRYPOINT ["java", "-jar", "app.jar"]



# Use lightweight JDK base image
FROM eclipse-temurin:17-jdk-alpine

# Set working directory
WORKDIR /app

# Copy the JAR from the target directory
COPY target/*.jar app.jar

# Run the JAR
ENTRYPOINT ["java", "-jar", "app.jar"]

