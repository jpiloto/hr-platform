FROM eclipse-temurin:17-jdk

# Install Git
RUN apt-get update && apt-get install -y git

WORKDIR /app

# Clone the repo
RUN git clone https://github.com/jpiloto/hr-system.git .

# Build the app
RUN ./mvnw clean package -DskipTests

EXPOSE 8080

CMD ["java", "-jar", "target/hr-system.jar"]