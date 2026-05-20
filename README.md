# Flask App on Kubernetes

A Python Flask API containerised with Docker and deployed to Kubernetes.

## Features
- REST API with health check endpoint
- Dockerised with a minimal Python image
- Kubernetes deployment with 2 replicas
- Resource limits and readiness probe configured

## Tech Stack
- Python / Flask
- Docker
- Kubernetes (kubectl)

## Run with Docker
docker build -t flask-k8s-app .
docker run -p 5000:5000 flask-k8s-app

## Deploy to Kubernetes
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml