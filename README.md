# Kubernetes Project

This repository contains Kubernetes configuration files for a project involving MongoDB and a web application using MongoDB. The project includes the following files:

- `mongo-configmap.yaml`: A Kubernetes ConfigMap file for configuring MongoDB.
- `mongo-express.yaml`: A Kubernetes Deployment file for running a web-based MongoDB administration tool.
- `mongo.yaml`: A Kubernetes Deployment file for setting up a MongoDB instance.
- `mongodb-secret.yaml`: A Kubernetes Secret file for storing sensitive information, such as passwords.

## Prerequisites

Before you begin, ensure you have the following:

- Access to a Kubernetes cluster. You can use Minikube for local development or a cloud-based Kubernetes cluster.
- `kubectl` installed and configured to manage your cluster.
- Docker or a container registry to build and push container images if required.

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/k8s-proj.git
   cd k8s-proj
2. Apply the folling commands
   
''' bash

kubectl apply -f mongo-configmap.yaml
kubectl apply -f mongo-express.yaml
kubectl apply -f mongo.yaml
kubectl apply -f mongodb-secret.yaml

kubectl get pods
kubectl get services
