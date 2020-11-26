# Raspberry Pi Demo

Build

```sh
docker build -t hello-http-world .
```

Publish

```sh
docker tag hello-http-world:latest dmitter/hello-http-world:latest
docker push dmitter/hello-http-world:latest
```

Run

```sh
docker run -d --name=hello-http-world --restart unless-stopped -p 8080:8080 dmitter/hello-http-world:latest
```

Update [more here](https://docs.docker.com/config/containers/start-containers-automatically/)

```sh
docker update --restart unless-stopped $(docker ps -q)
```

Stop and Remove

```sh
docker container stop <ID>
docker container rm <ID>
```
