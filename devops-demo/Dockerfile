# Güncel ve resmi Eclipse Temurin Java 17 JDK base image
FROM eclipse-temurin:17-jdk

# JAR dosyasını container'a kopyala
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

# Uygulamayı çalıştır (port 8080)
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "/app.jar"]