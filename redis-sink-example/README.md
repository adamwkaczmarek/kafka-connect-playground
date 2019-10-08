# Setup step by step

## Run docker containers

* `docker-compose up -d --build`

## Kafka Connect Workers configuration :

* `curl -s -X POST -H 'Content-Type: application/json' --data @datagen-config.json http://localhost:8088/connectors`

* `curl -s -X POST -H 'Content-Type: application/json' --data @redis-sink-config.json http://localhost:8088/connectors`
