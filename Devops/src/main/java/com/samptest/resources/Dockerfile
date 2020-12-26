FROM openjdk:8-jre-alpine
WORKDIR /app
COPY --from=build /devops/target/mavenIntergration-1.0-SNAPSHOT.jar /app
EXPOSE 8080
CMD ["java -jar mavenIntergration-1.0-SNAPSHOT.jar"]
