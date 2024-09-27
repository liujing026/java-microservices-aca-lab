# Build stage
FROM mcr.microsoft.com/openjdk/jdk:17-mariner
COPY spring-petclinic-my-service-3.2.5.jar app.jar
COPY ai.jar ai.jar
EXPOSE 8080

# Run the jar file
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-javaagent:/ai.jar","-jar","/app.jar"]

