# Curl Paste Docker

This docker container spins up;
* Node 8 [Alpine OS](https://www.alpinelinux.org/about/)
* Latest [rook2pawn/curl-paste](https://github.com/rook2pawn/curl-paste)


Image size 296MB 

## Docker Run: Quick start

```
docker run -d -p "80:8000" chasg/curl-paste
```

Done.


## Docker-compose: Getting Started

```
git clone https://github.com/chasgames/docker-curlpaste curlpaste && cd $_
docker-compose up -d
```


## Configuring

Service runs on port 8000 internally

Binded to port 80 by default.

Supports traefik for frontend proxy / https.

"data" folder is created so pastes can persist through upgrades.

## Upgrade

```
docker-compose build --no-cache
docker-compose up -d
```




#### Todo
Configurable expire time through environment variable

