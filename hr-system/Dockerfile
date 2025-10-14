FROM eclipse-temurin:17-jdk

WORKDIR /app

RUN git clone https://github.com/jpiloto/hr-system.git .

RUN ./mvnw clean package -DskipTests

EXPOSE 8080

CMD ["java", "-jar", "target/hr-system.jar"]