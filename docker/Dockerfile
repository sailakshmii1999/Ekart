# Use a base image with Java 17
FROM openjdk:17-jdk-slim

# Expose the port the application will run on
EXPOSE 8070

# Set the application home environment variable
ENV APP_HOME=/usr/src/app

# Create the working directory
WORKDIR $APP_HOME

# Copy the application JAR file into the container
COPY target/shopping-cart-0.0.1-SNAPSHOT.jar app.jar

# Set the entry point to run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
