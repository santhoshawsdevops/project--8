**Full-Stack Kubernetes Monitoring & Observability Platform
Overview**

This project implements a Kubernetes-based monitoring and observability environment using Minikube, Prometheus, Grafana, Node Exporter 
and Alertmanager.

The objective is to monitor Kubernetes workloads and infrastructure resources, visualize metrics through Grafana dashboards,
configure threshold-based alerts, and perform load testing to observe system behavior under traffic.

!!!!!!!!!!Project Architecture!!!!!!!!!!!!!



                    AWS EC2 Ubuntu
                         │
                         ▼
                    Minikube
                         │
              ┌──────────┴──────────┐
              │                     │
              ▼                     ▼
       Kubernetes App          Node Exporter
              │                     │
              │                     ▼
              │                 CPU / RAM
              │                 Disk / Network
              │                     │
              └──────────┬──────────┘
                         ▼
                    Prometheus
                         │
              ┌──────────┴──────────┐
              │                     │
              ▼                     ▼
           Grafana              Alertmanager
              │                     │
              ▼                     ▼
       Dashboards & Metrics    Email / Alerts





** Key Features:**
Deployed applications using Kubernetes Deployments and Services.
Created a local Kubernetes cluster using Minikube.
Configured Prometheus for metrics collection.
Integrated Node Exporter for infrastructure metrics.
Created Grafana dashboards for monitoring.
Configured CPU and resource-based alert rules.
Configured Alertmanager for alert notification management.
Performed HTTP load testing using ApacheBench.
Monitored system behavior during increased request traffic.
Troubleshot Kubernetes, Prometheus and Grafana configuration issues.
