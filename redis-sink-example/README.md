# Simple Kafka Connect example
In this example we will generating mock data using DataGen and streaming them to Redis (using Kafka Connect Redis).

# Setup

## Run docker containers

* `docker-compose up -d --build`

## Configure connectors

* `curl -s -X POST -H 'Content-Type: application/json' --data @datagen-config.json http://localhost:8088/connectors`

* `curl -s -X POST -H 'Content-Type: application/json' --data @redis-sink-config.json http://localhost:8088/connectors`
