1. Run "01_kafka_kraft_random_uuid_gen.bat" and generate a random uuid
2. Copy the generated UUID to "02_kafka_kraft_format_log_storage.bat"
3. Run "02_kafka_kraft_format_log_storage.bat"
    - format the kafka log storage
    - Running the second script with the UUID will format log storage
      and you would see the kraft-combined-logs sub-folder within logs folder
4. Run "03_kafka_server_start.bat" to start the kafka BROKER in kraft mode
    - notice the new folder _cluster_metadat-0 sub-folder within logs,
      which is the major change introduced within Kafka,
      and now the cluster metadata resides within the broker
5. Open a new Terminal
6. Propose a new topic name in place of <TOPIC_NAME>
    - Example : KRAFT-DEMO
7. Run "05_kraft_kafka_topic_create.bat" to create the TOPIC
8. Run "06_kafka_kraft_console_producer.bat" to create the PRODUCER
    - This will open the console producer within the Terminal and write some message to Produce
9. 


