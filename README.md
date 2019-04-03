The Application
==========


The application itself just contains functionality to register users. Users are stored in an In-Memory-Database.

- You can run the application using `mvn spring-boot:run`
- ...or you can run the WAR using `java -jar user-registration-application-0.0.1-SNAPSHOT.war`
- ...or you can deploy the WAR into a Servlet 3.0 compatible container such as Tomcat

The application uses Spring Boot. For the web interface Thymeleafe templates are used.

docker run -d --name sonarqube -p 9000:9000 -v sonar_home:/opt/sonarqube sonarqube:7.7-community  

mvn sonar:sonar -Dsonar.host.url=http://localhost:9000 -Dsonar.login=b40ba81da41465f49639ad2436319cc00e8ee079

2. docker build -t user-registration-application:1.0 .
3. docker run -p 9080:9080 user-registration-application:1.0
