# Guide
## docker
```shell
docker run -v ./conf:/usr/local/etc/redis --name some-redis -d redis redis-server --save 60 1 --loglevel warning
```
## docker-compose
```shell
docker-compose up -d
```