# Kubernetes & Minikube
Deploying MongoDB & Mongo Express using Kubernetes Minikube.

## Table of contents
* [About](#about)
* [Demo](#demo)
* [Installation](#installation)

## About
In this repo, we are going to build images and deploy MongoDB and Mongo-Express using Kubernetes [Minikube](https://minikube.sigs.k8s.io/docs/).


## Demo 
Check out the demo:
<p align="center"><img src="https://github.com/nekoemperor/mongo-kubernetes/blob/master/images/mongo-kubernetes.gif" width="768"  />

## Installation
* Install [Docker](https://docs.docker.com/get-docker/), Minikube and Kubectl [Minikube](https://minikube.sigs.k8s.io/docs/).
* Clone this repo
* In the terminal, go to the root folder of this repo
* Check if docker, minikube and kubectl are installed already by running this in terminal:
  - For Docker: ```docker```
  - For Kubernetes CLI: ```kubectl```
  - For Minikube: ```minikube```, ```minikube start``` and ```minikube status```, then run these:   
* ```kubectl apply -f mongo-secret.yaml``` 
* ```kubectl apply -f mongo.yaml```
* ```kubectl apply -f mongo-configmap.yaml```
* ```kubectl apply -f mongo-express.yaml```  
* ```minikube service mongo-express-service```
* click the URL, e.g., ```http://127.0.0.1:40089``` or ```http://192.168.49.2:30000``` which is generated in the terminal for opening the service default/mongo-express-service.
