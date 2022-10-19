This project seeks to make adding new domains to NGINX a matter of config when bringing up containers.

https://hub.docker.com/r/jwilder/nginx-proxy

When creating containers:
- With `docker run` use -e VIRTUAL_HOST="domain.com"
- with compose use:
```yml
    environment:
      - VIRTUAL_HOST: domain.com
```