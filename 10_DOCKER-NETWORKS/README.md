# DOCKER NETWORKS

## Introduction

You need to know that docker-compose uses a dedicated bridge network for a docker-compose.yml file

0. Some commands

```
docker describe 769f624cfb1f # get informations about a container
docker network ls # list our networks
docker network inspect 67140b76e5a7 # get informations about a network (even container working inside)
```

1. We will create or own network

``` 
docker network create maalsi-nancy
```

2. We will start a container within this network

``` 
docker run -d -p 80:80 -p 443:443 --name reverse_caddy --network maalsi-nancy caddy
```
