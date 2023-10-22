# Spring Boot + Apache Kafka + Handling live stream

## The Project

This is multi-module maven project demonstrates Apache Kafka in Spring Boot application
- Create Kafka Topic, Producer and Consumer
- Exchange simple String messages between Producer and Consumer using Kafka broker
- Exchange JSON messages between Producer and Consumer using Kafka broker

## Setup
#### Requirements
- Java 17
- Spring Boot 3.x
- Apache Kafka 2.13
    - https://kafka.apache.org/quickstart
- Maven 3.x
- Junit 5.x

## The Solution
- Implemented microservices in Spring Boot talking to Kafka as messaging solutions.
- This project contains two Spring Boot microservices 'kafka-producer-wikimedia' and 'kafka-consumer-database'
- EventStream is a web service that exposes continuous streams of structured event data.
- This project reads realtime stream data events from "https://stream.wikimedia.org/v2/stream/recentchange" in microservice 'kafka-producer-wikimedia' and send those events to the consumer microservice 'kafka-consumer-database'
