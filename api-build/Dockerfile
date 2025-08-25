FROM amazoncorretto:21-alpine

# Create app directory
WORKDIR /app

# Copy JAR from target folder into container
COPY demo-app.jar app.jar

# Expose app port
EXPOSE 8080

# Run the app
ENTRYPOINT ["java", "-jar", "app.jar"]
