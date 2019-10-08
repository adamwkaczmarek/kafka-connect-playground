Connectors configuration :

curl -s -X POST -H 'Content-Type: application/json' --data @datagen-config.json http://localhost:8088/connectors

curl -s -X POST -H 'Content-Type: application/json' --data @redis-sink-config.json http://localhost:8088/connectors

curl -s -X GET  -H 'Content-Type: application/json' http://localhost:8088/connectors