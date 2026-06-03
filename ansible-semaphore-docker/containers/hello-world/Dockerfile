# Step 1: Use an official JDK runtime as a parent image
FROM eclipse-temurin:17-jre

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy the executable JAR file from your host to the container
# Note: Adjust the source path if your JAR name or build folder is different
COPY target/*.jar app.jar

# Step 4: Expose the port your Spring Boot app runs on (default is 8080)
EXPOSE 8080

# Step 5: Run the JAR file
ENTRYPOINT ["java", "-jar", "app.jar"]