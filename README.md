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

Java code-:

package com.swapna.springbootdemo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@SpringBootApplication
public class SpringbootDemoApplication {

	public static void main(String[] args) {
		SpringApplication.run(SpringbootDemoApplication.class, args);
	}

}
@RestController
class HelloController {

	@GetMapping("/")
	public String index() {
		return "Greetings from Swapna & Welcome to Spring Boot World!";
	}

}
Run the Application:
./mvnw spring-boot:run
on terminal -curl http://localhost:8080

& also type on browser http://localhost:8080
Done!
