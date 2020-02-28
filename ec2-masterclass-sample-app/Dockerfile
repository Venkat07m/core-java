From openjdk:8
copy ./target/ec2-masterclass-sample-app-0.0.1-SNAPSHOT.jar ec2-masterclass-sample-app-0.0.1-SNAPSHOT.jar
CMD ["java", "-jar", "/ec2-masterclass-sample-app-0.0.1-SNAPSHOT.jar"]

HEALTHCHECK --interval=5s \
            --timeout=5s \
            CMD curl -f http://127.0.0.1:4567 || exit 1

RUN usermod -a -G docker jenkins
USER jenkins
chmod 777 /var/run/docker.sock

EXPOSE 4567
