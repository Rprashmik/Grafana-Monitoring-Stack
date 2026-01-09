# 📊 Grafana Monitoring, Logging & Alerting Stack

## 🚀 Project Overview

This project demonstrates a complete production-grade monitoring, logging and alerting system using:

- Prometheus
- Grafana
- Loki
- Promtail
- Blackbox Exporter
- Node Exporter
- Windows Exporter
- cAdvisor

It monitors:

- Linux Servers
- Windows Servers
- Docker Containers
- Websites / APIs
- Centralized Logs
- Sends Email Alerts

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
    
THIS IS TEST LINE

🧰 Tech Stack

Monitoring: Prometheus, Grafana

Logging: Loki, Promtail

Exporters: Node Exporter, Windows Exporter, cAdvisor, Blackbox Exporter

Containerization: Docker & Docker Compose

📈 Features

Linux server monitoring (CPU, RAM, Disk, Network)

Windows server monitoring

Docker container monitoring

Website uptime, latency and SSL monitoring

Centralized log monitoring using Loki

Email alerting for:

High CPU usage

Website down

Docker container down

📂 Project Structure
Grafana-Monitoring-Stack/
├── docker-compose.yml
├── prometheus.yml
├── Linux_Servers.yml
├── Windows_server.yml
├── blackbox/
├── loki/
├── promtail/
├── grafana-data/
├── loki-data/
├── screenshots/
└── README.md

▶️ How to Run
docker compose up -d


Open:

Grafana: http://localhost:3001

Prometheus: http://localhost:9090

📸 Dashboards

Add screenshots in the screenshots/ folder:

Linux server dashboard

Windows server dashboard

Docker containers dashboard

Website monitoring dashboard

Loki logs dashboard

🚨 Alerts Implemented

CPU usage > 80%

Website down

Docker container down

Alerts are sent using Grafana Email Alerting




  
