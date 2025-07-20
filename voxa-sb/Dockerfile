FROM maven:3.9.6-eclipse-temurin-17 AS build
WORKDIR /app

COPY pom.xml .
RUN mvn dependency:go-offline

COPY src ./src
RUN mvn clean package -DSkipTests

FROM openjdk:17-jdk-slim

WORKDIR /app

COPY --from=build /app/target/Voxa-0.0.1-SNAPSHOT.jar .

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "/app/Voxa-0.0.1-SNAPSHOT.jar"]