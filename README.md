# RabbitMQ Cluster Docker

Setup a RabbitMQ Cluster environment on your device using the pure [RabbitMQ](https://hub.docker.com/_/rabbitmq/) official docker image with Docker Compose.

## Features

- Super easy setup, config and expand
- Use a purely official RabbitMQ image
- Support latest version, optimized for Erlang cookie config
- Build-in HAProxy load balancing

## Quick start

```
docker compose up
```

Open http://localhost:15672 to login RabbitMQ dashboard.

> Username: `guest`  
> Password: `guest`

## Configuration

### `docker-compose.yml`

Docker [compose](https://docs.docker.com/compose/compose-file/) config file, including 3 RabbitMQ service cluster in the same network 

| Service     | Description               |
| ----------- | ------------------------- |
| `rabbitmq1` | RabbitMQ (cluster)        |
| `rabbitmq2` | RabbitMQ (cluster member) |
| `rabbitmq3` | RabbitMQ (cluster member) |
