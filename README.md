
# Development

create docker image and create and start container

```
    docker-compose up
```

stop and remove containers

```
    docker-compose down
```

update docker image and create/create and start container

```
    docker-compose up --build
```

alternitively if you want to use docker

build docker image from Dockerfile.dev

```
  docker build -f Dockerfile.dev -t IMAGETAG .
```

create and start container with volume

```
  docker run -it -p PORT:3000 -v /app/node_modules -v $(pwd):/app IMAGETAG
```

# Production

```
    docker build .
```

```
    docker run -p PORT:80 IMAGEID
```
