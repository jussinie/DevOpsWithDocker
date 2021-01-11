FROM openjdk:latest
COPY /spring-example-project /springapp
WORKDIR /springapp
RUN ./mvnw package
CMD java -jar ./target/docker-example-1.1.3.jar
