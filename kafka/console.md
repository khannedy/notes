## Create topic

``` bash
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic test
```

## List topic

``` bash
bin/kafka-topics.sh --list --zookeeper localhost:2181
```

## Produce message

``` bash
bin/kafka-console-producer.sh --broker-list localhost:9092 --topic test
```

## Consume message

``` bash
bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning
```

## Descript topic

``` bash
bin/kafka-topics.sh --describe --zookeeper localhost:2181 --topic my-replicated-topic
```
