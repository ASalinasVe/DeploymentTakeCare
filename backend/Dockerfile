# Usamos una imagen ligera de Java 17 (o la versión que uses)
FROM eclipse-temurin:17-jdk-alpine

# Definimos el directorio de trabajo
WORKDIR /app

# Copiamos el archivo .jar que generaste con Maven
# Asegúrate de que el nombre coincida con el que tienes en la carpeta target
COPY target/*.jar app.jar

# Exponemos el puerto que usa Spring Boot
EXPOSE 8080

# Comando para ejecutar la aplicación
ENTRYPOINT ["java", "-jar", "app.jar"]