# springBootMVCDocker

First please see that you can make it work without docker:

- pull the code
- go to pom.xml directory
- apply "mvn clean install"
- apply "java -jar target/templatejsp-0.0.1-SNAPSHOT.war"
- open browser and localhost:8080
- see welcome page
- go to terminal and apply CTRL+C to stop spring boot

Containerize It:

- apply "./mvnw install dockerfile:build"
- apply "docker run -p 8080:8080 -t springio/templatejsp"
- open browser and localhost:8080
- see welcome page


in order to stop:

- go to another terminal
- docker ps
- docker stop <containerId>

