FROM openjdk:8-jre-alpine
WORKDIR /app
EXPOSE 8080
COPY /mavenJobs/target/mavenIntergration-1.0-SNAPSHOT.jar app/demo.jar
ENTRYPOINT ["java","-jar","app/demo.jar"]
