FROM openjdk:8-jre-alpine
WORKDIR /app
EXPOSE 8080
COPY --from=  /target/*.jar  app/demo.jar
ENTRYPOINT ["java","-jar","app/demo.jar"]
