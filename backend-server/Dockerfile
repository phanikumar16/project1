# Use an official Maven image as the base image
FROM maven:3.8-openjdk-11-slim

# Set the working directory
WORKDIR /app

# Copy your Maven project into the container
COPY . /app

# Check Java version
RUN java -version

# Run Maven to build the project
RUN mvn clean install

# Expose the port your app will run on (optional, based on your app)
EXPOSE 8080

# Command to run your application (adjust based on your app)
CMD ["java", "-jar", "target/backend-server-1.0-SNAPSHOT.jar"]
