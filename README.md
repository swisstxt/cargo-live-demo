# Cargo Demo

## Python Application

This is a simple python flask application.

Create pipenv Virtual Environment for application dependencies:
```bash
pipenv install
```

To run the application locally use:

```bash
pipenv run server
```

## Docker Container

To build and publish the container use:

```bash
docker build . -t joschi36/cargo-demo:latest
docker push joschi36/cargo-demo:latest
```


## Kubernetes Deployment

Deploy on Kubernetes

```bash
kubectl apply -f kubernetes.yaml
```