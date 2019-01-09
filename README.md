# AMQP-Comunication-Proove-of-Concept
AMQP-RPC Comunication Proove of Concept using RabbitMQ and DotNet Core

## Running with Docker
1. Create a RabbitMQ docker container.

`$ docker run -d --hostname my-rabbit --name some-rabbit -e RABBITMQ_DEFAULT_USER=admin -e RABBITMQ_DEFAULT_PASS=admin -p 8080:15672 -p 5672:5672 rabbitmq:3-management`

2. Make sure that RabbitMQ server credentials are correct.

3. Create the images via `docker build`

4. Test to see behavior

    - Run many `Send` instances
    - Run many `Receive` instances
    - Remove all `Receive` instances and run them again

5. Enjoy