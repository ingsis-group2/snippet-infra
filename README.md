# snippet-infra
## How to use
### Run the following commands
```bash
docker login ghcr.io
## for master
docker compose -f docker-compose.master.yml up --build
## for dev
docker compose -f docker-compose.dev.yml up --build
```
