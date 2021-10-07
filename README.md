# docker-compose/minikube comparison/demo

This repo has config to run a simple webapp + database pair using either
docker-compose or minikube.

## docker-compose

To run this, install docker-compose, and run:

```sh
cd dc-feedback
docker-compose up
```

## minikube

To run this, install minikube/helm, and run:

```sh
cd helm-feedback
helm upgrade feedback . --atomic --install --debug \
 -f values.yaml \
 -f secrets.yaml
```
