### Kafka Environment setup with [Docker](https://www.docker.io/)

If you are using a Mac follow the instructions [here](https://docs.docker.com/installation/mac/) to setup a docker environment.

- Follow the development environment setup instruction [here](https://github.com/tq1/br-tq1-development)
- Start a kafka shell
    - `./start-kafka-shell.sh <Docker Ip> <Zookeeper>`, example `./start-kafka-shell.sh 192.168.59.103:9092 192.168.59.103:2181`
- From within the shell, create a topic
    - `$KAFKA_HOME/bin/kafka-topics.sh --create --topic my-node-topic --partitions 2 --zookeeper $ZK --replication-factor 1`

- For more details and troubleshooting see [https://github.com/wurstmeister/kafka-docker](https://github.com/wurstmeister/kafka-docker)
