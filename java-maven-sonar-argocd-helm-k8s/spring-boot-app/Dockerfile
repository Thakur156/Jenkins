# You can change this base image to anything else
# But make sure to use the correct version of Java (this is a java app and java image used to run java file we can 
# use maeven here by installing but we use it in jekins file docker as a agent
FROM adoptopenjdk/openjdk11:alpine-jre

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
