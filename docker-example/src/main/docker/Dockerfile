FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD docker-example-0.0.1-SNAPSHOT.jar docker-example.jar
RUN sh -c 'touch /docker-example.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/docker-example.jar"]