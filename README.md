# 🔐 Docker and Kubernetes Secrets with BusyBox Pods

## 📌 Project Overview
This project demonstrates how to securely manage **sensitive data** in Kubernetes using **Secrets**.  
We deploy two **BusyBox Pods** that retrieve a password from a Kubernetes Secret (`my-secret`) and print it at runtime.  

This is a **beginner-friendly example** to understand:
- How to create secrets in Kubernetes  
- How to consume them in Pods as **environment variables**  
- How to verify the secret value inside running containers  

---

## 🛠️ Technologies Used
- **Kubernetes (v1.20+)**
- **kubectl CLI**
- **BusyBox** (alpine lightweight Linux image)
- **Docker Desktop / Minikube / K3s** (any Kubernetes environment)

---

![Screenshot](assests/)
