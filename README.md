# Low latency with c++/linux
topic-basic message processing

# Demo
A multiple-producer/multiple-consumer system.
Input would be messages of different topics. Consumers will process the messages by topics.
Messages with same topic must be produced by the same producer and consumed in chronological order.

# Notation:
[Raw data] - this is the input at the very begining. It can contain multiple [Message].
[Message] - this is the basic input. A [Message] must contain a [Topic].
[Topic] - this is the key for message processing queue.
[Producer] - to generate/receive [Raw data]. It extracts [Raw data] into [Message] and put to corresponding [Message Queue]
[Consumer] - to process [Message] from [Message Queue]. Processed [Message] are put to [Distributor].
[Distributor] - to distribute processed [Message]. The destination may be network, file, output message queue, ...
[Message Queue] - 
