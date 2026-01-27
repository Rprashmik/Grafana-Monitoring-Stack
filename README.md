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

It also supports:

- Email Alerts
- Uptime Monitoring
- Resource Monitoring

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
🧰 Tech Stack
Monitoring: Prometheus, Grafana

Logging: Loki, Promtail

Exporters: Node Exporter, Windows Exporter, cAdvisor, Blackbox Exporter

Containerization: Docker & Docker Compose


---

# ⚠️ VERY IMPORTANT RULES

1. Mermaid diagram **must end with**:




