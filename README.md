# SIT323-2025 Prac6C - Kubernetes Task

## Overview
This repository contains the configuration and steps to deploy an application using Kubernetes. This guide will help you interact with the deployed application by verifying pods and services and accessing the application through port-forwarding.

### Tools Used
- **Kubernetes**: Container orchestration platform.
- **Kubectl**: Command-line tool for interacting with the Kubernetes cluster.
- **Kubernetes Dashboard**: Web-based user interface to interact with the Kubernetes cluster.
- **Docker**: Containerization tool for building images.

---

## Interacting with the Deployed Application

### 1. **Verify that the Application is Running**

After deploying the application to your Kubernetes cluster, you can check the status of the pods and services using the following commands:

#### a. **Check Pods**

To verify that the pods are running, use the following command:

```bash
kubectl get pods
<img width="528" alt="image" src="https://github.com/user-attachments/assets/75856787-f078-4394-8f99-7eca42b003f5" />
kubectl get services
<img width="527" alt="image" src="https://github.com/user-attachments/assets/95e4e8dc-bbd6-471b-a521-4e0f91d9e131" />
kubectl port-forward service/kubernetes-dashboard 8080:443 -n kubernetes-dashboard
http://localhost:8080
<img width="1512" alt="image" src="https://github.com/user-attachments/assets/92354bc1-0685-4a83-a6e5-cf4c177959d1" />




