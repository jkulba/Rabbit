# Rabbit
Useful Docker project that demonstrates the configuration of the message broker using a definitions file.  

## Usage
To start the docker container use:
```
$ docker-compose up
```
To view the configuration of a running instance of RabbitMQ us:
```
curl --silent --user admin:admin --header "Content-type: application/json" http://127.0.0.1:15672/api/definitions | jq . | tee config.json
```
To run generic instance of rabbitmq without the definitions use:
```
docker run --rm -it --hostname malina -p 15672:15672 -p 5672:5672 rabbitmq:3-management
```
To view the web console navigate to: http://localhost:15672/

Use username: guest password: guest



