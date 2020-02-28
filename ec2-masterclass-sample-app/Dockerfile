From openjdk:8

CMD ["java", "-jar", "/ec2-masterclass-sample-app-0.0.1-SNAPSHOT.jar"]

HEALTHCHECK --interval=5s \
            --timeout=5s \
            CMD curl -f http://127.0.0.1:4567 || exit 1

EXPOSE 4567
