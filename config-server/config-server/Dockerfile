# For Java 17, try this
FROM openjdk:17
# Refer to Maven build -> finalName
ARG JAR_FILE=target/*.jar
# cd /opt/app
WORKDIR /opt/app
# cp target/spring-boot-web.jar /opt/app/app.jar
COPY ${JAR_FILE} app.jar
#EXPOSE 8762
# java -jar /opt/app/app.jar
ENTRYPOINT ["java","-jar","app.jar"]