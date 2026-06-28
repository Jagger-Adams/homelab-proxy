# Reverse Proxy

Shared nginx reverse proxy fronting all self-hosted apps.

## Setup
1. `docker network create web` (one-time)
2. `docker compose up -d`
3. Each app joins the `web` network and adds a `conf.d/<app>.conf`.

Certs (Certbot) and secrets are gitignored