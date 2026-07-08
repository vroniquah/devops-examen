FROM eclipse-temurin:17-jdk-alpine as builder

WORKDIR /app

COPY . .
RUN sed -i 's/\r$//' mvnw
RUN chmod +x mvnw
RUN ./mvnw clean package -DskipTests

FROM eclipse-temurin:17-jre-alpine

WORKDIR /app

EXPOSE 8080

COPY --from=builder /app/target/*.jar app.jar

ENTRYPOINT ["java", "-jar", "/app/app.jar"]
