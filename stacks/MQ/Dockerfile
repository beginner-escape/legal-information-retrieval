FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install -y openjdk-11-jdk

COPY ./confluent-community-7.1.2.tar.gz ./confluent-community-7.1.2.tar.gz
COPY ./supervisord ./supervisord
RUN tar -xvf ./confluent-community-7.1.2.tar.gz

ENV CONFLUENT_HOME="/confluent-7.1.2"
ENV PATH=.:$PATH:$CONFLUENT_HOME/bin

CMD sh ./supervisord