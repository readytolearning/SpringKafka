# SpringKafka
SpringKafka

1.Download kafka.
2. Start zookeeper
bin\windows\kafka-server-start.bat config\server.propertiesbin\windows\kafka-server-start.bat config\server.properties

3. Start Kafka
bin\windows\kafka-server-start.bat config\server.properties

4.Create Topic
kafka-topics.bat --create --topic first-topic --partitions 4 --replication-factor 1 --zookeeper localhost:2181
5.start consumer
kafka-console-consumer.bat --topic first-topic --bootstrap-server localhost:9092

6. Start local spring boot application.
7 hit the rest service
http://localhost:8080/pvc-kafka/producer?message=test

8.We can able to see messages in consumer.
