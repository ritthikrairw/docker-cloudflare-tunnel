# docker-cloudflare-tunnel

This is a Cloudflare tunnel docker-compose for self host applications.

Service included

## Installation

1. Copy the `.env.example` file to `.env`
2. Config the `.env` file

```env
# App Information
APP_NAME=cloudflare-tunnel      # Application name (for config the container name)
```

3. After set the `.env` run command `docker compose up -d`
4. Connect the container by run command `docker exec -it <container-name or ID> bash`
5. Login the cloudflare by run command `cloudflared tunnel login` and open link on browser
6. Create tunnel by run command `cloudflared tunnel create <NAME>`
7. Edit a `config.yml` in `/root/.cloudflared`
8. Route the dns by run command `cloudflared tunnel route dns <UUID or NAME> <hostname>`
9. Start the tunnel by run command `cloudflared tunnel run <UUID or NAME>`


> Don't forget to link network between container

