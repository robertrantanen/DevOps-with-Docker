FROM openjdk:8-alpine

WORKDIR /app

COPY . /app

RUN ./mvnw package && adduser -D app && chown -R app: /app

USER app

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
