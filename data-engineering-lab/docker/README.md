# PostgreSQL stack with Docker Compose

A local PostgreSQL database with pgAdmin, plus a Python job that downloads a CSV from [datos.gov.co](https://www.datos.gov.co) and loads it into the database. Everything runs in containers, so the only requirement is Docker.

## Run it

```bash
cp .env.example .env      # set your own passwords
docker compose up -d      # starts PostgreSQL, pgAdmin and the load job
```

- pgAdmin: http://localhost:5050
- PostgreSQL: `localhost:5432`

## Structure

| Path | Purpose |
|---|---|
| `docker-compose.yml` | Services, named volume and shared network |
| `.env.example` | Credentials template (the real `.env` is never committed) |
| `ingest/` | Dockerfile and Python script for the CSV load |

## Dataset

| | |
|---|---|
| Source | |
| Rows loaded | |
| Table | |

## Design notes

- 
