| NAME               | ID         | ADVPROG CLASS |
| ------------------ | ---------- | ------------- |
| Sultan Ibnu Mansiz | 2306275840 | B             |

# Module 9: Software Architecture - Reflection

## 1. What is ***amqp***?
AMQP, or Advanced Message Queuing Protocol, is a messaging standard designed for asynchronous communication between applications. It facilitates dependable message transmission, efficient routing, and service decoupling, making it well-suited for distributed systems.

## 2. What does it mean *guest:guest@localhost:5672*, what is the first `guest`, and what is the second `guest`, and what is `localhost:5672` is for?
The initial `guest` refers to the username required for authentication with the RabbitMQ server, while the second `guest` represents the corresponding password. The notation `localhost:5672` specifies the local machine's address (`localhost`) and the designated port (`5672`) for connecting to the RabbitMQ server.

---

### Slow Subscriber Simulation
![SlowSimulation](images/SlowSubs.png)
The chart shows a spike in published messages (yellow) followed by successful delivery and acknowledgment. At this moment, the message queue is empty, with no messages in 'Ready' or 'Unacked' state. This indicates that the subscriber successfully consumed all published messages without backlog.

    
