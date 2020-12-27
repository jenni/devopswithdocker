FROM openjdk:8-jdk

WORKDIR /usr/app

COPY .mvn .mvn
COPY src src
COPY mvnw mvnw
COPY mvnw.cmd mvnw.cmd
COPY pom.xml pom.xml

RUN ./mvnw package
EXPOSE 8080

CMD java -jar ./target/docker-example-1.1.3.jar