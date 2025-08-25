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

![Screenshot 1](assets/Screenshot%20(190).png)
![Screenshot 2](assets/Screenshot%20(191).png)
![Screenshot 3](assets/Screenshot%20(194).png)

![Screenshot 4](assets/Screenshot%20(198).png)
![Screenshot 5](assets/Screenshot%20(199).png)
![Screenshot 6](assets/Screenshot%20(200).png)
