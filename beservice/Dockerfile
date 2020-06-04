FROM openjdk:11.0.4-jre
LABEL APP_ID="beservice"
VOLUME /app
EXPOSE 8080
ENTRYPOINT java -Xdebug -Xrunjdwp:transport=dt_socket,address=*:8000,server=y,suspend=n -jar /app/$JAR