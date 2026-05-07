# ☸️ Multi-Cluster Kubernetes Disaster Recovery System

## 🚀 Overview

This project demonstrates a Multi-Cluster Kubernetes Disaster Recovery Architecture using Docker, Flask, and Kubernetes.

The system contains:

* Primary Cluster (cluster-a)
* Backup Cluster (cluster-b)

If the primary cluster goes down, the backup cluster continues serving traffic.

---

## 🧰 Tech Stack

* Kubernetes
* Minikube
* Docker
* Flask
* Kubernetes Services
* Port Forwarding

---

## 🌍 Architecture

### Cluster A

Primary production cluster

### Cluster B

Backup disaster recovery cluster

---

## 🚀 Features

* Multi-cluster setup
* High availability foundation
* Disaster recovery simulation
* Dockerized Flask backend
* Kubernetes Deployments
* Kubernetes Services
* Port forwarding access
* Failover testing

---

## 💥 Disaster Recovery Demo

### Cluster A URL

http://localhost:9090

### Cluster B URL

http://localhost:9191

When Cluster A is stopped:

* Cluster A becomes unavailable
* Cluster B continues serving traffic

---

## 📦 Deployment

### Apply Kubernetes manifests

```bash
kubectl apply -f k8s-manifests/
```

### Port forward

```bash
kubectl port-forward service/backend-service 9090:5000
```

---

## 👨‍💻 Author

Rishu Raj
