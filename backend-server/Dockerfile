# Use an official Maven image with OpenJDK 8
FROM maven:3.8.1-openjdk-8

# Set the working directory
WORKDIR /app

# Copy the pom.xml and the source code into the container
COPY pom.xml .
COPY src ./src

# Run Maven to build the project
RUN mvn clean install

# Expose a port if your application needs to run (adjust based on your app)
EXPOSE 8080
