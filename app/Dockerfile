FROM openjdk:11-jdk-slim
VOLUME /tmp
ADD app/target/docker-to-aws-with-java-0.0.1-SNAPSHOT.jar app.jar
#add vai pegar o que est? na pasta/target/ e vai copiar para dentro do container
EXPOSE 8080
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/app.jar",]
#ENTRYPOINT s?o linha de comandos para serem executadas na cria??o do container
