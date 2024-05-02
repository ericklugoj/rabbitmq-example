# Rabbitmq NodeJS Example

a very basic example (kind of `hello world`) using NodeJS rabbitmq in monorepo.

## Requirements

- pnpm installed
- Docker (recommended)
- RabbitMQ Server running in localhost _(with default config)_

> [!TIP]
> use Docker to run RabbitMQ easily:
>
> docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.13-management

## Quick start

Start RabbitMQ server (from docker is recommended)

Install dependencies

```console
pnpm install
```

Start consumer

```console
pnpm run start:consumer
```

Start producer _(in another console tab)_

```console
pnpm run start:producer
```

a message from producer should be showed in consumer console tab.
