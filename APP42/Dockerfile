FROM ubuntu:18.04
RUN apt update
RUN apt install -y  default-jdk
RUN apt install -y tomcat9
RUN apt install -y maven 
RUN apt install -y git 
RUN git clone https://github.com/Stupin87/App42.git
WORKDIR /home/keglia/
WORKDIR /home/keglia/App42
RUN mvn clean package
RUN mv /home/keglia/App42/target/App42PaaS-Java-MySQL-Sample-0.0.1-SNAPSHOT.war /usr/local/tomcat/webapps

