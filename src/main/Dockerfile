FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD demoServices-0.0.1-SNAPSHOT.jar demoServices.jar
RUN sh -c 'touch /demoServices.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /demoServices.jar" ]
