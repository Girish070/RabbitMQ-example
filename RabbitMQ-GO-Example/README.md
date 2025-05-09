# RabbitMQ Go Example

This project demonstrates a simple message queue system using **RabbitMQ** with **Go**. It includes both a **producer** that sends messages and a **consumer** that receives them.

## Features

- Simple producer-consumer model
- Uses RabbitMQ for message brokering
- Written in Go (Golang)

## Prerequisites

- [Go](https://golang.org/doc/install) 1.18 or later
- [RabbitMQ](https://www.rabbitmq.com/download.html) server running locally or remotely

### Install RabbitMQ (if not already installed)

Using Docker:
```bash
docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3-management
RabbitMQ Dashboard: http://localhost:15672

Default login: guest / guest

Project Structure
bash
Copy
Edit
.
├── consumer.go   # Consumes messages from the queue
├── producer.go   # Sends messages to the queue
How to Run
Start RabbitMQ (make sure it's running)

Run the Consumer (in one terminal)

bash
Copy
Edit
go run consumer.go
Run the Producer (in another terminal)

bash
Copy
Edit
go run producer.go
You should see messages being sent and received between the producer and consumer via RabbitMQ.

Queue Info
Queue Name: hello

Exchange: default (empty)

Routing Key: hello

License
This project is open-source and available under the MIT License.

yaml
Copy
Edit

---

Would you like me to include setup instructions for deploying this with Docker or Kubernetes as well?
