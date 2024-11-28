# Traefik (Docker Swarm)

## Requirements

- `direnv`
- `1password`

## Deploy

Copy `.envrc.dist` to `.envrc` for direnv to use:

```shell
cp .envrc.dist .envrc
```

Then allow direnv to load environment variables with 

```shell
direnv allow
```

Then deploy the stack using :

```shell
docker stack deploy -c docker-compose.traefik.yml traefik
```