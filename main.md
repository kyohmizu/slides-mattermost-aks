class: center, middle, blue
# Deploy Mattermost on AKS

---
### whoami

.left-small[
    ![image](https://pbs.twimg.com/profile_images/994762110792953856/EheEvqBY_400x400.jpg)
]

.right-large[
- Kyohei Mizumoto(@kyohmizu)

- C# Software Engineer

- Interests
    - Docker/Kubernetes
    - Go
    - Security
]

---
### Source

<u><https://github.com/kyohmizu/mattermost-aks></u>

- Database isn't included

  - Need to create Database earlier

---
### Configuration

- Azure Kubernetes Service (AKS)

- Kubernetes resources

  - Mattermost

  - Prometheus

  - Grafana

- Azure Load Balancer

- Azure Database for PostgreSQL server

---
### Tools

- Terraform

  - Cluster configuration management

- Helm

  - Template engine

---
class: center, middle, blue
# Demo

---
### Step

1. Create AKS cluster

2. Deploy kubernetes resources

3. Grafana settings

---
### future prospects

- Logging

  - fluentd

- Continuous Delivery

  - Spinnaker/Tekton

- Service Mesh

  - Istio/SMI

- Database configuration management

---
class: center, middle, blue
# Thank you!
