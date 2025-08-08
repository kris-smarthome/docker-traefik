# docker-traefik
Traefik reverse proxy with Cloudflare DNS resolver and Letsencrypt.

## usage
Clone this repository to your local machine, edit the config file to match your environment, and run docker compose.

```bash
git clone https://github.com/kris-smarthome/docker-traefik.git traefik/
cd traefik
nano .env
docker compose up -d
```

> [!NOTE]
> Create a Cloudflare token, copy the value into .env. Also, create the traefik network before deploying this stack: `docker network create -d bridge traefik`. 