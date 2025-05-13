- Name: Janssen Benedict
- Class: Pemrograman Lanjut A
- NPM: 2306152102

### a. How much data your publisher program will send to the message broker in one run?
The publisher program sends five messages to the message broker in one run.

### b. The url of: "amqp://guest:guest@localhost:5672" is the same as in the subscriber program, what does it mean?
The URL of "amqp://guest:guest@localhost:5672" is the same as in the subscriber program, meaning that both the publisher and the subscriber are communicating by connecting to the same RabbitMQ broker, with the broker running locally on the default port for AMQP. This ensures that both the publisher and the subcriber can exchange messages through a shared message queue on the same RabbitMQ broker.

![alt text](ScreenshotPublisher1.png)

<br><br>After running both the publisher and the subscriber, the publisher program sent five messages or events through the message broker. The subscriber then processes these five messages or events that were sent.
![alt text](ScreenshotPublisher2.png)

<br><br>The spike in the RabbitMQ chart shows the rate of the messages that were sent to the channel within a specific interval of time. By running the publisher and making it send messages to the message broker, it resulted in their being a spike in the chart, indicating that messages were successfully published and received by the RabbitMQ broker.
![alt text](ScreenshotPublisher3.png)