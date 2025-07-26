## Apache Kafka

|English Sentence|Chinese Sentence|
|--|--|
|A producer sends messages to Kafka; a consumer retrieves those messages from Kafka and processes them.|`中文表达（标准说法）`: 生产者将消息发送到 Kafka，消费者从 Kafka 中拉取这些消息并进行处理。<br> 在 Kafka 里，生产者负责把消息“写进去”，而消费者负责把消息“读出来”并做相应的处理。|
|Kafka needs to create a topic with multiple partitions. Then, each message has a key, which Kafka uses to determine which partition the message should go to.|`中文表达（标准说法）`: Kafka 需要先创建一个包含多个分区的主题，然后每条消息都会带有一个 key，Kafka 会根据这个 key 将消息路由到对应的分区。<br> 在 Kafka 中，我们通常会创建一个主题（topic）并设置多个分区（partition），当生产者发送消息时，如果这条消息带有 key，Kafka 就会根据这个 key 的哈希值来决定将消息放到哪个分区里，以保证相同 key 的消息会进入同一个分区。|
|We need to create a Kafka topic with multiple partitions.|我们需要创建一个 Kafka 主题，并配置多个分区。|
|Each message can have a key to determine which partition it goes to.|每条消息可以带一个 key，Kafka 会根据 key 来决定分区。|
|Messages with the same key will go to the same partition.|拥有相同 key 的消息会被发送到同一个分区。|
|A producer sends messages to Kafka.|生产者会将消息发送到 Kafka。|
|A consumer polls messages from Kafka and processes them.|消费者会从 Kafka 拉取消息并进行处理。|
|The consumer group ensures load balancing across multiple consumers.|消费者组可以实现多个消费者之间的负载均衡。|
|Kafka guarantees message order within a partition.|Kafka 保证在同一个分区内的消息顺序。|
|We are using Kafka to decouple services.|我们使用 Kafka 来解耦服务之间的依赖。|
|The offset tracks how far the consumer has read.|Offset 表示消费者当前读取到的位置。|
|We need to persist the consumer offset.|我们需要持久化消费者的 offset。|
|Kafka is used for real-time data streaming.|Kafka 用于实时数据流处理。|
|We are scaling by increasing the number of partitions.|我们通过增加分区数来实现扩展。|
|Messages are temporarily stored in Kafka before being processed.|消息会先暂存在 Kafka 中，然后再被处理。|
|The Kafka broker is responsible for managing partitions and topics.|Kafka broker 负责管理分区和主题。|
|We should monitor the lag between the producer and consumer.|我们需要监控生产者和消费者之间的延迟（lag）。|
|Kafka can act as a buffer to handle traffic spikes.|Kafka 可以作为缓冲区来应对流量高峰。|
|We use schema registry to manage message formats.|我们使用 schema registry 来管理消息格式。|
|The consumer rebalance happens when a new consumer joins or leaves the group.|当有新的消费者加入或离开消费者组时，会发生 rebalance。|
|We use Kafka in combination with databases like PostgreSQL or MongoDB.|我们会把 Kafka 和数据库（比如 PostgreSQL 或 MongoDB）结合使用。|
