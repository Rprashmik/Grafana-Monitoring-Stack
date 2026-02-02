# 📊 Grafana Monitoring, Logging & Alerting Stack

> 🚀 Production-Grade Monitoring, Logging & Alerting Stack using Prometheus, Grafana & Loki

---


🚀 Project Overview

This project demonstrates a complete, production-grade monitoring, logging, and alerting stack built using modern observability tools:

Prometheus

Grafana

Loki

Promtail

Blackbox Exporter

Node Exporter

Windows Exporter

cAdvisor

🔍 It monitors:

Linux servers

Windows servers

Docker containers

Websites / APIs

Centralized logs

⚡ It also supports:

Email alerts

Uptime monitoring

Resource monitoring

---

## 🏗️ Architecture

```mermaid
flowchart TB
    A["Servers / Apps / Containers<br/>Linux, Windows, Docker, Websites"] --> B["Exporters<br/>Node, Windows, cAdvisor, Blackbox, Promtail"]
    B --> C["Prometheus"]
    B --> D["Loki"]
    C --> E["Grafana"]
    D --> E["Grafana"]
    E --> F["Dashboards & Alerts<br/>Email Notifications"]
```

## 🧰 Tech Stack

- **Monitoring:** Prometheus, Grafana  
- **Logging:** Loki, Promtail  
- **Exporters:** Node Exporter, Windows Exporter, cAdvisor, Blackbox Exporter  
- **Containerization:** Docker & Docker Compose  

---

## 📈 Features

- Linux server monitoring (CPU, RAM, Disk, Network)  

- Windows server monitoring  

- Docker container monitoring  

- Website uptime, latency, and SSL monitoring  

- Centralized log monitoring using Loki  

- Email alerting for:
  - High CPU usage  
  - Website down  
  - Docker container down  

---
📧 Alerting & Notifications

This monitoring stack includes fully functional, production-ready email alerting implemented using Grafana + Alertmanager.

🚨 Implemented Alerts

🔥 High CPU Usage (> 80%)

🌐 Website Down (Blackbox Exporter)

🐳 Docker Container Down

🖥️ Server Unreachable

📬 Notification Channel

Email (SMTP)

🧪 Tested Scenarios

Stopping Docker containers

Shutting down exporters / servers

Generating high CPU load

✅ Alerts are delivered to email in real-time with clear FIRING and RESOLVED states.

---
## 📂 Project Structure

Grafana-Monitoring-Stack/
├── docker-compose.yml
├── prometheus.yml
├── Linux_Servers.yml
├── Windows_servers.yml
├── alertmanager.yml
├── rules.yml
├── blackbox/
├── loki/
├── promtail/
├── templates/
├── grafana-data/
├── loki-data/
├── screenshots/
└── README.md


---

## ▶️ How to Run
📸 Screenshots
🚨 Alerts Implemented
🧪 Tested Environment
👨‍💻 Author


---

## 📸 Screenshots

### 🐧 Linux Server Monitoring
![Linux](screenshots/Linux-dashboard.png)

### 🪟 Windows Server Monitoring
![Windows](screenshots/Windows-dashboard.png)

### 🐳 Docker Monitoring
![Docker](screenshots/Docker-dashboard.png)

### 📜 Loki Logs (Docker Containers)
![Loki](screenshots/Loki-dashboard.png)


### 📜 Loki Logs (System /var/log)

![Loki](screenshots/Varlogs-loki-dashboard.png)

### 🌐 Website Monitoring (Blackbox)
![Blackbox](screenshots/Blackbox-dashboard.png)

### 📧 Alert Email (Grafana + Alertmanager)
![Alert](screenshots/alert-email.png)

---


Start the stack using Docker Compose:

```bash
docker compose up -d
Open in your browser:

Grafana: http://monitor.deployflow.tech/

Prometheus: http://192.168.0.190:9090

📸 Dashboards
Screenshots are available in the screenshots/ folder:

Linux server monitoring dashboard

Windows server monitoring dashboard

Docker containers monitoring dashboard

Website monitoring dashboard (Blackbox)

Loki logs dashboard

🚨 Alerts Implemented
CPU usage > 80%

Website down

Docker container down

Alerts are sent using Grafana Email Alerting.

🧪 Tested Environment
Ubuntu / Debian Linux

Docker & Docker Compose

Windows Server with windows_exporter

👨‍💻 Author
Rashmik Parmar
DevOps Engineer
