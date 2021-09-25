# Kafka-Docker-Container
Setting Up Apache Kafka Using Docker

Step 1:
Clone file to your local.

Step 2:
run the command below
docker-compose up

for running deamen
docker compose up -d 

Step 3:
docker exec -it [container-id] /bin/sh

Step 4:
Create a topic
$ bin/kafka-topics.sh --create --topic quickstart-events --bootstrap-server localhost:9092

Step 5:
for produce data
$ bin/kafka-console-producer.sh --topic quickstart-events --bootstrap-server localhost:9092
this is first message

Step 6:
for consume data
$ bin/kafka-console-consumer.sh --topic quickstart-events --from-beginning --bootstrap-server localhost:9092

