# Usa una imagen base de OpenJDK con Gradle
FROM eclipse-temurin:21-jdk AS builder

# Configura el directorio de trabajo
WORKDIR /app

# Copia los archivos de build de Gradle
COPY gradlew .
COPY build.gradle .
COPY settings.gradle .
COPY gradle/ ./gradle/
COPY src/ ./src/

# Construye la aplicación
RUN chmod +x gradlew && ./gradlew bootJar

# Imagen final
FROM eclipse-temurin:21-jre

# Copia el jar del contenedor de construcción
COPY --from=builder /app/build/libs/*.jar app.jar

# Define el puerto
EXPOSE 8761

# Ejecuta el jar
ENTRYPOINT ["java", "-jar", "/app.jar"]
