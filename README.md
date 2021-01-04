# docker-warm-up

```
docker run hello-world

docker create hello-world

docker start container-id

docker start -a container-id

docker ps

docker ps --all - LISTING ALL THE CONTAINERS

docker -v

docker version
```

```
docker run busybox ls

docker system prune - DELETING ALL THE DATA AND RUNNING CONTAINERS

docker logs container-id
```

```
docker stop id - TAKES 10 SECS, IF NOTHING HAPPENS WITHIN THIS 10 SEC, THEN KILL COMMAND EXECUTION

docker kill id - IMMEDIETLY KILLS THE RUNNING PROCESS

docker exec -it container-id command

docker exec -it container-id sh - FOR SHELL COMMAND ACCESS

docker run -it busybox sh

```

```
# Use an existing docker image as a base

FROM alpine

# Download and install a dependency

RUN apk add --update redis

# Second Step

RUN apk add --update gcc

# Tell the image what to do when it starts as a container

CMD ["redis-server"]

docker build

docker run container-id
```

```
docker build -t shohan494/redis-starter:latest .
```

What one point I am intentionally missing is the section of manually building image

```
docker run -p 8080:8080 shohan494/simpleweb
```

# docker-compose warm-up
```
docker-compose up
docker-compose up -d
docker-compose down
docker-compose up --build
docker-compose ps
```

