# docker-terraria-tmodloader

A docker attempt to bootstrap a terraria server with tModloader


## Deployment

### Application

```sh
docker build -t terraria .
docker run -it --name=terraria \
--restart="always" \
-p 7777:7777 \
-v "/path/to/config/":/root/.local/share/Terraria/ModLoader \
terraria:latest
```
