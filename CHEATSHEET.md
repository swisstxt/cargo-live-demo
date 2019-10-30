# Cargo Presentation Cheatsheet

## 0. Preperations

Browser with following open Tabs
- http://127.0.0.1:8088
- http://127.0.0.1:7070
- https://hub.docker.com/r/joschi36/cargo-demo
- http://livedemo-cargo.swisstxt.ch

## 1. Show Python Program

Go through the app.py program

## 2. Show Pipfile and Dependencies

Needed dependencies: flask and redis

## 3. Run Server

```sh
pipenv run server
# or
pipenv run python app.py
```

Open first Browser Window

## 4. Create Dockerfile

Go through Dockerfile

## 5. Build and Tag Docker Image

```sh
docker build . -t joschi36/cargo-demo:latest
```

There are other Container Registries

## 6. Run Docker Image

```sh
docker run -p 7070:8088 joschi36/cargo-demo:latest
```

## 7. Run Docker Image with Env Var

```sh
docker run -p 7070:8088 -e NAME="Cloud Meetup" joschi36/cargo-demo:latest
```

## 8. Push Dockerfile

```sh
docker push joschi36/cargo-demo:latest
```

Push to Docker, other Providers quay, GCR, github package registry, selfhosted.

## 9. First Kubernetes Deployment

- Namespace _(Project)_
- Deployment _(Container deployment)_
- Service _(Cluster availability)_
- Ingress _(HTTP Internet availability)_

## 10. Redis Kubernetes Deployment

- add. Redis Deployment
- add. Redis Service

## 11. Redis Persistance

- add. Redis PVC
- change Redis Deployment
