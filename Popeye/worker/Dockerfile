FROM maven:3.9.6-eclipse-temurin-21-alpine as builder

COPY . .


RUN mvn dependency:resolve

RUN mvn package


FROM eclipse-temurin:21-jre-alpine

WORKDIR /target

COPY --from=builder /target .

CMD java -jar worker-jar-with-dependencies.jar