From openjdk:8

copy /var/lib/jenkins/workspace/Job1/ec2-masterclass-sample-app/target/currency-exchange-service-0.0.1-SNAPSHOT.jar currency-exchange-service-0.0.1-SNAPSHOT.jar
CMD ["java","-jar","currency-exchange-service-0.0.1-SNAPSHOT.jar"]

HEALTHCHECK --interval=5s \
            --timeout=5s \
            CMD curl -f http://127.0.0.1:4567 || exit 1

EXPOSE 4567
