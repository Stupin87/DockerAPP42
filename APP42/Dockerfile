FROM openjdk:8-jdk-alpine
COPY src /App42/src
COPY pom.xml /App42
WORKDIR /home/keglia/App42
RUN apt install -y maven
RUN mvn clean package
EXPOSE 8080
CMD ["java", "-jar", "App42PaaS-Java-MySQL-Sample-0.0.1-SNAPSHOT.war"]

