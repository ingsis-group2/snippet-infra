# snippet-infra
## How to use
### Run the following commands
```bash
docker login ghcr.io
## for master
docker compose -f docker-compose.master.yml pull
docker compose -f docker-compose.master.yml up --build
docker compose -f docker-compose.master.yml run --rm certbot certonly --webroot --webroot-path /var/www/certbot/ -d tista.duckdns.org
## for dev
docker compose -f docker-compose.dev.yml pull
docker compose -f docker-compose.dev.yml up --build
docker compose -f docker-compose.dev.yml run --rm certbot certonly --webroot --webroot-path /var/www/certbot/ -d tista-dev.duckdns.org
```