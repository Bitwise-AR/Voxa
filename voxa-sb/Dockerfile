# Use a base image with Java 17 (or your project's Java version)
FROM eclipse-temurin:24-jdk-jammy

# Set the working directory inside the container
WORKDIR /app

# Copy the Maven wrapper files (if you use them, good practice)
COPY mvnw .
COPY .mvn .mvn

# Copy the pom.xml and build it to download dependencies
COPY pom.xml .
RUN ./mvnw dependency:go-offline

# Copy the rest of the application source code
COPY src src

# Build the Spring Boot application
# -DskipTests is important to skip tests during the build
RUN ./mvnw clean install -DskipTests

# Expose the port your Spring Boot application runs on (default is 8080)
EXPOSE 8080

# Define the command to run your application
# Replace 'your-app-name.jar' with the actual name of your generated JAR file.
# You can find this in your pom.xml under <build><finalName> or it's usually artifactId-version.jar
ENTRYPOINT ["java", "-jar", "target/Voxa-0.0.1-SNAPSHOT.jar"]