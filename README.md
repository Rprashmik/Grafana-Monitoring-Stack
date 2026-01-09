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




  
