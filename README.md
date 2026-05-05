## 🚀 GitOps Observability Platform



# This project demonstrates a complete \*\*end-to-end DevOps pipeline\*\* using modern cloud-native tools. It covers CI/CD, GitOps deployment, Kubernetes, monitoring, visualization, and real-time alerting.

# 

---

# 

# \## 🧠 Project Overview

# 

# In real-world systems, deploying an application is not enough. We must also automate deployments, monitor performance, detect failures, and alert teams.

# 

# This project implements all of these in a single workflow.

# 

# \---

# 

# \## 🔄 Complete Workflow

# 

# ```

# Developer → GitHub → GitHub Actions → Docker Hub → Argo CD → Kubernetes

# → Prometheus → Grafana → Slack Alerts

# ```

# 

# \### Explanation

# 

# \- Code is pushed to GitHub

# \- GitHub Actions builds and pushes Docker image

# \- Argo CD detects changes and deploys to Kubernetes

# \- Prometheus collects application metrics

# \- Grafana visualizes metrics

# \- Alerts are triggered and sent to Slack

# 

# \---

# 

# \## 🛠️ Tech Stack

# 

# | Category | Tool |

# |---|---|

# | Cloud | AWS EC2 |

# | Containerization | Docker |

# | Orchestration | Kubernetes (k3s) |

# | GitOps | Argo CD |

# | CI/CD | GitHub Actions |

# | Monitoring | Prometheus |

# | Visualization | Grafana |

# | Alerting | Slack Webhooks |

# | Backend | Python Flask |

# 

# \---

# 

# \## ⚙️ Features

# 

# \- Automated CI/CD pipeline

# \- GitOps-based deployment

# \- Kubernetes application deployment

# \- Real-time monitoring

# \- Custom metrics using `/metrics`

# \- Grafana dashboards

# \- Slack alert notifications

# 

# \---

# 

# \## 🏗️ Architecture

# 

# ```

# GitHub (Code)

# ↓

# GitHub Actions (CI/CD)

# ↓

# Docker Hub (Image)

# ↓

# Argo CD (GitOps)

# ↓

# Kubernetes (k3s on EC2)

# ↓

# Prometheus (Metrics)

# ↓

# Grafana (Dashboards + Alerts)

# ↓

# Slack (Notifications)

# ```

# 

# \---

# 

# \## 📸 Screenshots

# 

# \### 🔹 Argo CD Deployment

# !\[Argo CD](https://github.com/Sathish11-Design/gitops-observability-platform/blob/main/Images/Argo%20CD.png)

# 

# \### 🔹 Kubernetes Pods Running

# !\[Kubernetes Pods](https://github.com/Sathish11-Design/gitops-observability-platform/blob/main/Images/Kubernetes%20Pods.png)

# 

# \### 🔹 GitHub Actions CI/CD Pipeline

# !\[GitHub Actions](https://github.com/Sathish11-Design/gitops-observability-platform/blob/main/Images/GitHub%20Actions%20CICD.png)

# 

# \### 🔹 Grafana Dashboard

# !\[Grafana Dashboard](https://github.com/Sathish11-Design/gitops-observability-platform/blob/main/Images/Grafana%20Dashboard.png)

# 

# \### 🔹 Prometheus Targets

# !\[Prometheus Targets](https://github.com/Sathish11-Design/gitops-observability-platform/blob/main/Images/Prometheus%20Targets.png)

# 

# \### 🔹 Alert Firing in Grafana

# !\[Alert Firing](https://github.com/Sathish11-Design/gitops-observability-platform/blob/main/Images/Alert%20Firing.png)

# 

# \### 🔹 Slack Alert Notification

# !\[Slack Alert](https://github.com/Sathish11-Design/gitops-observability-platform/blob/main/Images/Slack%20Alert%20Message.png)

# 

# \---

# 

# \## 🚨 Alerting Logic

# 

# Alert triggers when:

# 

# ```

# Error rate > 1% OR high number of failed requests

# ```

# 

# \*\*PromQL Example:\*\*

# 

# ```promql

# sum(increase(flask\_http\_request\_duration\_seconds\_count{status!="200"}\[5m]))

# ```

# 

# \---

# 

# \## 📊 Dashboard Panels

# 

# \- API Request Rate

# \- Request Duration

# \- HTTP Status Codes

# \- Pod CPU Usage

# \- Pod Memory Usage

# \- Pod Restarts

# 

# \---

# 

# \## 🧪 How to Run Locally

# 

# ```bash

# git clone https://github.com/Sathish11-Design/gitops-observability-platform.git

# cd gitops-observability-platform

# 

# docker build -t task-manager-api .

# docker run -p 5000:5000 task-manager-api

# ```

# 

# \---

# 

# \## 📌 Key Learnings

# 

# \- Implemented GitOps workflow using Argo CD

# \- Built CI/CD pipeline with GitHub Actions

# \- Integrated application metrics with Prometheus

# \- Designed real-time dashboards in Grafana

# \- Configured alerting with Slack integration

# \- Deployed scalable app on Kubernetes

# 

# \---

# 

# \## 💼 Resume Highlights

# 

# \- Built a GitOps-based Kubernetes deployment system

# \- Implemented end-to-end CI/CD pipeline

# \- Designed observability platform with Prometheus \& Grafana

# \- Configured real-time Slack alerting for incidents

# \- Deployed infrastructure on AWS EC2

# 

# \---

# 

# \## 🚀 Future Improvements

# 

# \- Add logging using Loki

# \- Implement auto-scaling (HPA)

# \- Use Terraform for infrastructure provisioning

# \- Add Ingress with custom domain

# 

# \---

# 

# ⭐ If you found this useful, give it a star!



