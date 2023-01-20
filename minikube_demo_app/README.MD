# Project title
- React & MongoDB on Minikube(kubernetes)

## Installation
- Install Minikube
- Install Docker or VM for Minkube's engine
- Start Docker 
- `minikube start --driver docker` to start with Docker as the engine
- `d` to see the application

## Usage
- Run `minikube ssh docker pull mongo:5.0` to install mongo
- Run `kubectl apply -f mongo-config.yaml` to create for the first time or update the mongo-config.yaml in the cluster
- Run `kubectl apply -f mongo-secret.yaml` to create for the first time or update the mongo-secret.yaml in the cluster
- Run `kubectl apply -f mongo-mongo.yaml` to create for the first time or update the mongo.yaml in the cluster
- Run `kubectl apply -f mongo-webapp.yaml` to create for the first time or update the webapp.yaml in the cluster
- Run `minikube service webapp-service` to see the application
- `kubectl get all` to see information on deployments, pods and services.
- Run `minikube ip` to see your ip address of your node.

## Changelog

## Bugs
- To access the web application, the command `minikube service webapp-service` has to be used for tunneling which assigns its url to http://127.0.0.1:57026. Not the node's external ip address and port which is http://<'next available ip in your subnet'>:30100.



