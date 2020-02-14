# graylog-docker

### docker install 
```
curl -fsSL https://get.docker.com -o get-docker.sh;
chmod +x  get-docker.sh;
sh get-docker.sh;
usermod -a -G docker $USER;
docker version;
```

### docker-compose install
```
curl -fsSL https://github.com/docker/compose/releases/download/1.25.4/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose;
chmod +x /usr/local/bin/docker-compose;
docker-compose version;
```
[DOCKER-COMPOSE](https://github.com/docker/compose/releases)

### ctop install

```
curl -fsSL https://github.com/bcicen/ctop/releases/download/v0.7.3/ctop-0.7.3-linux-amd64 -O /usr/local/bin/ctop;
chmod +x /usr/local/bin/ctop;
ctop -v
```
[CTOP](https://github.com/bcicen/ctop)

## 
```
mkdir -p {mongo_data,es_data,graylog_journal}
chown -R 999.999 mongo_data
chown -R 1000.1000 es_data
chown -R 1000.1000 graylog_journal
```
