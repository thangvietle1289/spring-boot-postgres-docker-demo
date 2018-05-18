FROM openjdk:8-jre
WORKDIR /docker-demo
VOLUME ["/docker-demo"]
COPY maven/spring-boot-postgres-docker-demo.jar spring-boot-postgres-docker.jar
RUN sh -c 'touch spring-boot-postgres-docker.jar'
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "spring-boot-postgres-docker.jar"]
