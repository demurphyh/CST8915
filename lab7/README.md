# CST8915 Lab 7

## Youtube Walkthrough Link

[youtube link](https://youtu.be/S-ELPXWEnXA)

## Written analysis of the RabbitMQ configuration issues

### Whether RabbitMQ is a stateless or stateful application

- RabbitMQ is a stateful application.

### The implications of running RabbitMQ without persistent storage

- Running RabbitMQ without persistent storage means that RabbitMQ cannot save it's state between restarts.

### What happens when the RabbitMQ pod is deleted or restarted

- If the RabbitMQ pod is deleted or restarted then all of the data will be deleted and data loss will occur.

### Potential solutions to this problem (research-based)

- In order to solve this problem we can either run the RabbitMQ bean with persistent storage or make sure that RabbitMMQ backs up messages frequently.

### Does using Azure Service Bus solve the issues identified with RabbitMQ Configuration in this Lab?

- If we use Azure Service Bus it will automatically persist our data between restarts and solve the issue that this labs RabbitMQ configuration has.
