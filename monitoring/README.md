# traefik-demo

Demo of stack for monitoring composed by:

* traefik
* prometheus
* grafana

## Requirements

* [docker-compose](https://docs.docker.com/compose/install/)

## How to run

## export variables or have these set in the environment
```
export ROOT_URL=http://grafana:3000
export DEFAULT_INSTANCE_NAME=grafana
export ADMIN_USER=admin
export ADMIN_PASSWORD="beans&rice"
export GF_SECURITY_ADMIN_USER=admin
export GF_SECURITY_ADMIN_PASSWORD="beans&rice"
export GF_USERS_ALLOW_SIGN_UP=false
```

### To load

```bash
docker-compose up
```

### To complete reload

```bash
docker-compose stop && docker-compose rm && docker-compose up -d --build
```

### To access Traefik

[http://localhost:8088](http://localhost:8088)

### To access Prometheus

[http://localhost:9090](http://localhost:9090)

### To access Grafana

[http://localhost:3000](http://localhost:3000)

|user|password|
|---|---|
|admin|admin|

## Grafana Configuration

### DataSource Config

![alt text](https://i.imgur.com/j4Vdseb.png)

### Dashboard Import

![alt text](https://i.imgur.com/xHxBLgx.png)
