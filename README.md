# Raspberry Pi Demo

Build

```sh
docker build -t dmitter/rpi-http-server:latest .
```

Publish

```sh
docker push dmitter/rpi-http-server:latest
```

Run

```sh
docker run -d --restart unless-stopped dmitter/rpi-http-server:latest
```
