# Rabbit

Generic usage of docker-compose with RabbitMQ

curl --silent --user admin:admin --header "Content-type: application/json" http://127.0.0.1:15672/api/definitions | jq . | tee config.json

docker run --rm -it --hostname malina -p 15672:15672 -p 5672:5672 rabbitmq:3-management
