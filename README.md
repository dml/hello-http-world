# Raspberry Pi Demo

Build

```sh
docker build -t rpi-http-server .
```

Publish

```sh
docker tag rpi-http-server:latest dmitter/rpi-http-server:latest
docker push dmitter/rpi-http-server:latest
```

Run

```sh
docker run -d --name=rpi-http-server --restart unless-stopped -p 8080:8080 dmitter/rpi-http-server:latest
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
