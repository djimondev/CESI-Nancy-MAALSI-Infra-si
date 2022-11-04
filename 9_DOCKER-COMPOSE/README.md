# DOCKER-COMPOSE

## Install docker-compose

Just follow the steps [here](https://docs.docker.com/compose/install/)

## somme commands

```bash
docker-compose up # run our container stack
docker-compose up -d # run our container stack in deamon mode
docker-compose logs -f # display logs of all containers of our stack
docker-compose logs -f www2 # display logs for 1 service
docker exec -ti b21051e809b4 sh # attach to the container console, the classic way
docker-compose exec www2 sh # attach to the container console, the 'docker-compose' way
docker-compose down # stop our container stack
```

## Lab 1

use this docker-compose.yml

```
version: "3"
services:
  www1:
    image: httpd
    ports:
      - "8001:80"
    volumes:
      - ./www1:/usr/local/apache2/htdocs/
  www2:
    image: caddy
    ports:
      - "8002:80"
    volumes:
      - ./www2:/usr/share/caddy/
  www3:
    image: nginx
    ports:
      - "8003:80"
    volumes:
      - ./www3:/usr/share/nginx/html/
```

## Lab 2

## Lab 3
