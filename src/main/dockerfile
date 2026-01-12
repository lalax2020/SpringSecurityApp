FROM eclipse-temurin:17-jdk

WORKDIR /app

COPY . .

RUN chmod +x ./gradlew
RUN ./gradlew clean build -x test -x check

EXPOSE 8080

CMD ["java", "-jar", "build/libs/demo-1.jar"]
