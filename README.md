# Simple Micro-services demo app on Docker

- [Introduction](#introduction)
- [Steps](#steps)
- [Detached Mode](#detached-mode)

Introduction
=============
The goal is to learn using Docker compose to configure docker containers for
each of the different micro-services for a demo product commerce app. Using a
single command docker compose will spin up all the containers with all the dependencies

Steps
=========

1. Start the docker containers

```bash
docker-compose up
```

> Docker compose creates a virtual network for all of the services (containers)
with the service name being the hostname of the dependency

2. Check product service at 

```
curl http://localhost:8080
```

3. Check website  at 

```
curl http://localhost:8081
```

Detached Mode
================

Docker compose can be run in detached mode

```
docker-compose up -d
```

Seeing the backgroup processes
```
docker-compose ps
```
Stoping the processes

```
docker-compose stop
```
 