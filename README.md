# n8n Docker

Simple Docker Compose setup for running **n8n**.

## Requirements

- Docker
- Docker Compose

## Run

```bash
docker compose up -d
```

Open: `http://localhost:5678`

## Stop

```bash
docker compose down
```

## Update

```bash
docker compose pull
docker compose up -d
```

## Fly.io

Create the persistent volume once before deploying:

```bash
fly volumes create n8n_data --size 1 --region ams
```

Then deploy with:

```bash
fly deploy
```
