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

1.Deployed applications using Kubernetes Deployments and Services.

2.Created a local Kubernetes cluster using Minikube.

3.Configured Prometheus for metrics collection.

4.Integrated Node Exporter for infrastructure metrics.

5.Created Grafana dashboards for monitoring.

6.Configured CPU and resource-based alert rules.

7.Configured Alertmanager for alert notification management.

8.Performed HTTP load testing using ApacheBench.

9.Monitored system behavior during increased request traffic.

10.Troubleshot Kubernetes, Prometheus and Grafana configuration issues.
