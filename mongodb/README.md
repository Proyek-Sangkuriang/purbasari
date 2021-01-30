# What is MongoDB?

> [MongoDB](https://www.mongodb.org/) is a cross-platform document-oriented database. Classified as a NoSQL database, MongoDB eschews the traditional table-based relational database structure in favor of JSON-like documents with dynamic schemas, making the integration of data in certain types of applications easier and faster.

Base image : Bitnami mongo with debian 10
Mongodb Version : 4.4

# Run from image

```console
$ docker run --name mongodb sangkuriang/mongodb:latest
```

## Run from Docker Compose

### Single node

```console
$ docker-compose up -d
```

### With replicas

```console
$ docker-compose up -d -f docker-compose-replicaset.yml
```

> All data will be stored in /data/db please change it in Docker-compose file to met your need.