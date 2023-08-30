# Springboot-Docker-image-project

Creating a Spring Boot application involves several steps. 

Access the Spring Initializr:
Go to the Spring Initializr website at https://start.spring.io/.

Configure Your Project:
Fill in the necessary details to configure your Spring Boot project:

Project Maven
Language JavaKotlinGroovy
Spring Boot (SNAPSHOT)3.1.33.0.11 
Project Metadata
Group com.swapna
Artifact springboot-demo
Name springboot-demo
Description Demo project for Spring Boot
Package name com.swapna.springboot-demo
Packaging Jar
Java 17
DependenciesADD -spring web
Generate the Project:
Click the "Generate" button to download a ZIP file containing your Spring Boot project's initial structure.

Unzip the Project:
Extract the downloaded ZIP file to a directory springboot-project

Open the Project in Your IDE:
Import the project into Vscode.


In the src/main/java/com/swapna/springbootdemo/SpringbootDemoApplication.java directory 

Run the Application:
./mvnw spring-boot:run
on terminal -curl http://localhost:8080

& also type on browser http://localhost:8080
Done!

created Dockerfile in springboot-demo folder
mvn clean pacage command- to create jar file inside target folder


docker build -t image-name:tag
docker run -p 8080:8080 image-name:tag
docker tag "docker image id" registry username/image name
docker push registry username/image name
