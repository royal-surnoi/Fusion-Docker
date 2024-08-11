FROM alpine/java:21-jdk

RUN mkdir -p /home/app

COPY . /home/app

WORKDIR /home/app

EXPOSE 8080

CMD ["nohup","java","-jar","FusionIQ-0.0.1-SNAPSHOT.jar","&"]