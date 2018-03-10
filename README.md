OpenJDK 8 and NodeJS 9 docker image
---

This container is used for ci server.  
Skip install openjdk8 and nodejs9, and build time is shorter.

# Getting started

## CircleCI
put this image name to .circleci/config.yml.

```
version: 2
jobs:
  build:
    docker:
      - image: takemikami/openjdk8-nodejs9:latest
```

## check image at local PC
view gcloud command usage.

```
$ docker pull takemikami/openjdk8-nodejs9
$ docker run -t openjdk8-nodejs9 java -version
$ docker run -t openjdk8-nodejs9 node -v
```
