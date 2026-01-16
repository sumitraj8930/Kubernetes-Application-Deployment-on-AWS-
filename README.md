
# **Kubernetes Application Deployment on AWS**

This project deploys two applications — an **NGINX static website** and a **Django Notes App** — on a Kubernetes cluster running on **AWS**. The setup uses **Docker** for containerization, **Kubernetes** for orchestration, and **Prometheus + Grafana** for monitoring.

---

## **📌 Tech Stack**

* **AWS (EC2, VPC, IAM)**
* **Docker**
* **Kubernetes**
* **NGINX**
* **Django**
* **Linux (Ubuntu)**
* **Prometheus & Grafana**
* **Ingress Controller**

---

## **📂 Project Overview**

The main goals of this project are:
✔ Deploy containerized web applications on a Kubernetes cluster
✔ Manage traffic using Kubernetes Ingress
✔ Build secure AWS infrastructure using VPC and IAM
✔ Enable monitoring using Grafana dashboards and Prometheus metrics

---

## **🚀 Deployment Steps (High-Level)**

1. **Provision AWS Infrastructure**

   * EC2 instance for Kubernetes
   * IAM role for EC2
   * VPC for secure networking

2. **Install Kubernetes**

   * kubeadm / minikube / kind (based on your setup)
   * Configure worker nodes (if multi-node)

3. **Containerize Apps**

   * Build Docker image for Django Notes App
   * Use public image for NGINX static website

4. **Deploy to Kubernetes**

   * Create Deployment and Service for both apps
   * Apply manifests using `kubectl`

5. **Configure Ingress**

   * Enable Ingress Controller
   * Route URLs:

     * `/` → NGINX website
     * `/notes` → Django app

6. **Monitoring Setup**

   * Install Prometheus for metrics
   * Install Grafana for dashboards

---

## **🔗 Application Routing**

| Path     | Service              |
| -------- | -------------------- |
| `/`      | NGINX Static Website |
| `/notes` | Django Notes App     |

---

## **📊 Monitoring**

* **Prometheus** scrapes metrics from Kubernetes
* **Grafana** visualizes:

  * Pod usage
  * Node CPU & Memory
  * Deployment health
  * Network metrics

---

## **🌐 Security & Networking**

* VPC used for network isolation
* IAM role for EC2 access management
* Kubernetes namespaces for logical separation

---
## **📌 Key Learnings**

✔ Containerization with Docker
✔ Kubernetes deployments & services
✔ Ingress-based routing
✔ Prometheus metrics & Grafana dashboards
✔ AWS cloud infrastructure & networking
✔ Application monitoring & observability


