# Keycloak Docker-Compose

This repository contains a docker-compose and all necessaries resources to deploy a Keycloak using Docker Images.
## Usage

You need to define the EXTERNAL_IP environment variable using the node ip address. This environment is necessary to JGROUPS cluster service discovery. Also, you need to set the database configurations on environment file, located on "environments/example/dev/.env".

```bash
$ EXTERNAL_IP=192.168.0.10 \
        APP_NAME=example \
        ENV=dev \
        docker-compose up -d
```
