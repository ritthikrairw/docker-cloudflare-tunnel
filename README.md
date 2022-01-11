# docker-cloudflare-tunnel

This is a Cloudflare tunnel docker-compose for self host applications.

## Installation

1. Run command `docker compose up -d`
2. Connect the container by run command `docker exec -it <container-name or ID> bash`
3. Login the cloudflare by run command `cloudflared tunnel login` and open link on browser
4. Create tunnel by run command `cloudflared tunnel create <NAME>`
5. Edit a `config.yml` in `/root/.cloudflared`
6. Route the dns by run command `cloudflared tunnel route dns <UUID or NAME> <hostname>`
7. Start the tunnel by run command `cloudflared tunnel run <UUID or NAME>`


> Don't forget to link network between docker container

