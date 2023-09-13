# Guide
## docker
```shell
docker run -p 13306:3306 --name some-mysql --ulimit nofile=262144:262144 -v ./data:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=123456 -d mysql:8.0
```
## docker-compose
```shell
docker-compose up -d
```