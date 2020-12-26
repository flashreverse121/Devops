FROM openjdk:8-jre-alpine
WORKDIR /app
EXPOSE 8080
ADD ./target/*.jar  app/demo.jar
ENTRYPOINT ["java","-jar","app/demo.jar"]
