[![Docker](https://img.shields.io/badge/containerized-Docker-blue)](https://www.docker.com/)
[![Deploy on AWS](https://img.shields.io/badge/deployed-AWS%20EC2-green)](https://aws.amazon.com/ec2/)
[![Grafana Monitoring](https://img.shields.io/badge/monitoring-Grafana-orange)](https://grafana.com/)

# Odilia Voting App – Full Docker Deployment (EC2 Edition)

This project contains the complete setup to deploy the Odilia Voting App using Docker Compose on AWS EC2, including monitoring with Grafana and Prometheus.

## 🔧 Services Included

- `yelb-ui`: Frontend web app
- `yelb-appserver`: Backend API
- `yelb-db`: PostgreSQL database
- `redis-server`: Primary Redis cache
- `prometheus`: Monitoring metrics collection
- `node-exporter`: Server metrics
- `grafana`: Dashboards and visualization

## 🚀 To Deploy

```bash
docker-compose up -d
```

## 🌐 Access URLs (EC2 IP: 3.82.195.93)

- App UI: http://3.82.195.93
- Grafana: http://3.82.195.93:3000 (default user/pass: admin/admin)
- Prometheus: http://3.82.195.93:9090
- Node Exporter: http://3.82.195.93:9100

## 📁 Structure

```
odilia-full-app/
├── docker-compose.yml
├── configs/
│   └── redis/
│       ├── redis.conf
│       └── sentinel.conf
└── monitoring/
    └── prometheus.yml
```

Ensure Docker and Docker Compose are installed before deploying.
