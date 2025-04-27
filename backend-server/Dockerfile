# Use an official Maven image from Docker Hub
FROM maven:3.8.4-openjdk-11-slim AS build

# Set the working directory inside the container
WORKDIR /app

# Copy your project files into the container
COPY . /app

# Run Maven to build the project
RUN mvn clean install

# Expose a port if your application needs to run (adjust based on your app)
EXPOSE 8080

# Define the command to run the application (if applicable)
CMD ["java", "-jar", "target/backend-server-1.0-SNAPSHOT.jar"]
