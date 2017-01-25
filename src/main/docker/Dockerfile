FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD spring-microservices-account-reg-1.1.0.RELEASE.jar  app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar accounts" ]
