# Docker compossimo

A docker image with composer and prestissimo

## Run

```shell
docker run --rm -it -v `pwd`/project:/app ypereirareis/compossimo install --ignore-platform-reqs --no-scripts
```

## Build

```shell
docker build -t ypereirareis/compossimo .
```

### Change default user id/group

```shell
docker build --build-arg USER_ID=1000 -t ypereirareis/compossimo .
```

### Change composer version

```shell
docker build --build-arg COMPOSER_VERSION=1.6.3 -t ypereirareis/compossimo .
```
