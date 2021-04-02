FROM openjdk:8-jdk-alpine

COPY Program.java /app/Program.java
WORKDIR /app
RUN [ "javac", "Program.java" ] 

CMD [ "java", "Program" ]