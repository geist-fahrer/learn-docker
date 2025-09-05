# Notes
- Host name to connect to host machine from a container is host.docker.internal
- Within same network containers can talk to each other using their names.
- There are different network drivers and bridge is default.

## Commands
```bash
docker network ls
docker network create fav-app-net
docker run -p 3000:3000 --rm --name fav-node --network fav-app-net favorite-node
docker run --name mongodb --network fav-app-net mongo
docker network create --driver bridge my-net
```
## Things to remember
