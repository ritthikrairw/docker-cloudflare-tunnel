# docker-cloudflare-tunnel

This is a Cloudflare tunnel docker-compose for self host applications.

## Installation

1. Connect the container by run command `docker exec -it <container-name or ID> bash`
2. Login the cloudflare by run command `cloudflared tunnel login` and open link on browser
3. Create tunnel by run command `cloudflared tunnel create <NAME>`
4. Edit a `config.yml` in `/root/.cloudflared`
5. Route the dns by run command `cloudflared tunnel route dns <UUID or NAME> <hostname>`
6. Start the tunnel by run command `cloudflared tunnel run <UUID or NAME>`


> Don't forget to link network between docker container

