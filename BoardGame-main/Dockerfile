# FROM adoptopenjdk/openjdk11
  
# EXPOSE 8080
 
# ENV APP_HOME /usr/src/app

# COPY target/*.jar $APP_HOME/app.jar

# WORKDIR $APP_HOME

# CMD ["java", "-jar", "app.jar"]


# Use OpenJDK as the base image
# Use an OpenJDK base image
FROM eclipse-temurin:17-jdk-jammy

# Set working directory inside container
WORKDIR /app

# Copy the JAR file from the build context (make sure the JAR name matches your build output)
COPY target/Boardgame-*.jar app.jar

# Expose the application port (change if needed)
EXPOSE 8080

# Run the app
ENTRYPOINT ["java", "-jar", "app.jar"]


