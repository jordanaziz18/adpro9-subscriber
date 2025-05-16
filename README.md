
### What is amqp?
- AMQP is an open standard protocol for message-oriented middleware, enabling reliable, secure, and platform-independent communication between clients and servers

### What does it mean? guest:guest@localhost:5672 , what is the first guest, and what is the second guest, and what is localhost:5672 is for? 

- The first guest is the username. The second guest is the password. localhost is the hostname (the server where the AMQP broker, like RabbitMQ, is running). 5672 is the port number used by the AMQP protocol (the default port for RabbitMQ). So, the string connects to an AMQP server running in the local machine, using the username guest and password guest.

Simulation slow subscriber
![image](https://github.com/user-attachments/assets/70947954-2a2c-4b68-bd9a-228735e6431c)

The publisher program sent 16 messages, indicating pending consumption. The number increased due to slow customer movement or slower publisher speed. The system processed the messages, indicating proper operation. The figure may vary depending on device speed or message volume.


Running at least three subscribers
![image](https://github.com/user-attachments/assets/be1baf58-de33-4382-9e4d-d812e27de1b0)

![image](https://github.com/user-attachments/assets/0baa47e2-c595-42cf-b570-165ec37bb458)
when running the RabbitMQ's event-driven system reduces processing time and queue spike by running multiple subscriber instances, distributing messages among them, and allowing parallel handling. This behavior is a core strength of event-driven systems, enabling horizontal scalability and a faster drop in message backlog as subscribers increase.


