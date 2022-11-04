# Docker

## Installation

Follow the documentation [here](https://www.docker.com/products/docker-desktop/)

## First commands

```bash
docker --version # see wich version of docker is installed
docker run --rm bash echo "Hello MAALSI NANCY" # run a container and display Hello MAALSI NANCY (and remove it)
docker ps # list running containers
docker stop $(docker ps -q) # stop every running containers
docker run --rm bash sleep 10 # run a containe during 10 seconds
docker ps -a # list stopped containers
docker system prune -a # remove every docker item
```

## Create our own image

See [Dockerfile_lab](./Dockerfile_lab/)

```


```
