\# HR Platform



This repo orchestrates the `hr-system` and `hr-payroll` microservices using Docker Compose. Each service dynamically pulls its source code during build, ensuring independence and production-grade architecture. Kafka is used for event-driven communication.



\## Services



\- `hr-system`: Produces Kafka events

\- `hr-payroll`: Consumes Kafka events

\- `Kafka` + `Zookeeper`: Messaging backbone



\## How to Run



```bash

docker compose up --build

