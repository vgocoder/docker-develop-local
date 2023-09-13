# Guide
## docker
```shell
docker run -d -p 18123:8123 -p 19000:9000 --name some-clickhouse-server
    -v ./ch_data:/var/lib/clickhouse
    -v ./ch_logs:/var/log/clickhouse-server 
    --ulimit nofile=262144:262144 
    clickhouse/clickhouse-server 
echo 'SELECT version()' | curl 'http://localhost:18123/' --data-binary @-
```
## docker-compose
```shell
docker-compose up -d
```