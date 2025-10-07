# 🚀 DevOps Internship Assessment – Next.js App Directory Version

### Objective
Containerize and deploy a Next.js (App Router) application using Docker, GitHub Actions, and Minikube.

---

### 🧠 Tech Stack
- Next.js 14+
- Docker
- GitHub Actions (CI/CD)
- Kubernetes (Minikube)



## Setup Instructions

### 1. Local Run

```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

### 2. Docker Run Locally

# Build image
```
docker build -t nextjswexaai .
```
# Run container
```
docker run -p 3000:3000 nextjswexaai
``` 

### 3. Deployment on Minikube
# Start Minikube
```
minikube start
```

# Apply Kubernetes manifests
```
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
``` 
# Check pods
```
kubectl get pods
``` 
# Check service
```
kubectl get svc
``` 

### 4. Access Deployed App

# Get Minikube IP
```
minikube ip
```
#### Open browser at http://<minikube-ip>:30001
