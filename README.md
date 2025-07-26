# 🗒️ Notes App – Kubernetes Deployment on AWS EC2

This project demonstrates deploying a **Notes App** containerized and running on a Kubernetes cluster hosted on an AWS EC2 instance.

---

## 🚀 Tech Stack

- App: Django Notes App
- Kubernetes: 1 Master + 3 Worker nodes
- Platform: AWS EC2
- Service Port: 8000 (NodePort)

---

## 📁 Project Structure

k8s-notes-app-ec2/
├── namespace.yaml # Kubernetes namespace manifest
├── deployment.yaml # Deployment manifest for the Notes app
├── service.yaml # Service exposing the app on port 8000
└── README.md # Project documentation

## ⚙️ How to Deploy

Make sure your Kubernetes cluster is up and running, then:

```bash
kubectl apply -f namespace.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

🌐 Access the app :
Open your browser and go to:
http://<your-ec2-public-ip>:8000
Replace <your-ec2-public-ip> with your actual EC2 instance's public IP address






