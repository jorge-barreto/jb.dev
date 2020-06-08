To run JB.dev and its subdomains in production, run the following from the manager node, with the compose file in scope:

```
docker swarm init --advertise-addr $HOST_IP
docker network create -d overlay webnet
docker-compose config | docker stack deploy --prune --compose-file - jb_dev
```

Before doing so, please ensure the presence of a local .env file with the relevant details.
