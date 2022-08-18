# Armadillo Docker File

In order to push to DockerHub, you need to log in first.

``` bash
docker login -u aidanprognos
Password:
Login Succeeded
```

To find the version to use, increment based on the latest in dockerhub.

see [Armadillo Docker Hub](https://hub.docker.com/r/prognosai/armadillo/tags)

## Build it

> docker build -t prognosai/armadillo:0.0.5 .

## Run it

> docker run -it prognosai/armadillo:0.0.5 sh

## Deploy it

> docker push prognosai/armadillo:0.0.5
