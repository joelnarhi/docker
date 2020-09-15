FROM openjdk:8-jdk
EXPOSE 8080
ADD spring-example-project .
RUN ./mvnw clean install
CMD java -jar ./target/docker-example-1.1.3.jar


