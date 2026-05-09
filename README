# Ansible monitoring infrastructure

Multi-host infrastructure project with automated deployment using Ansible.

## Stack

- Ubuntu Linux
- Python
- Flask
- Nginx
- Docker / Docker Compose
- Prometheus
- Node Exporter
- Grafana

# Infrastructure

| Host | Purpose                             |
| ---- | ----------------------------------- |
| vm1  | Nginx reverse proxy / load balancer |
| vm2  | Flask application                   |
| vm3  | Flask application                   |
| vm4  | Prometheus + Grafana                |

# Features

- Automated infrastructure deployment with Ansible
- Reverse proxy and load balancing with Nginx
- Multi-host architecture
- Docker-based services
- Prometheus monitoring
- Node exporter metrics
- Grafana dashboards

# Project structure

```bash
**.**

├── README

├── ansible.cfg

├── ansible.cfg.example

├── deploy.yml

├── **host_vars**

│   ├── vm1.yml

│   ├── vm2.yml

│   ├── vm3.yml

│   └── vm4.yml

├── inventory

├── inventory.example

└── **roles**

    ├── **app**

    │   ├── **files**

    │   │   ├── Dockerfile

    │   │   ├── compose.yml

    │   │   ├── main.py

    │   │   └── requirements.txt

    │   └── **tasks**

    │       └── main.yml

    ├── **docker**

    │   └── **tasks**

    │       └── main.yml

    ├── **monitoring**

    │   ├── **files**

    │   │   └── compose.yml

    │   ├── **tasks**

    │   │   └── main.yml

    │   └── **templates**

    │       └── prometheus.yml.j2

    └── **nginx**

        ├── **files**

        │   └── compose.yml

        ├── **tasks**

        │   └── main.yml

        └── **templates**

            └── default.conf.j2
```

# Deployment

## Clone repository

```bash
git clone https://github.com/shinshkaa/ansible-monitoring-infra.git
cd ansible-monitoring-infra
```

## Configure inventory

```bash
cp inventory.example inventory
```
Fill your hosts and SSH settings.

## Configure ansible.cfg

```bash
cp ansible.cfg.example ansible.cfg
```

## Run playbook

```bash
ansible-playbook deploy.yml
```
