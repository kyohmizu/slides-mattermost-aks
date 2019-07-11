class: center, middle, blue
# Deploy Mattermost on AKS

---
exclude: true
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

---

---
class: center, middle, blue
# Upgrade AKS Cluster

---
### Upgrade AKS Cluster

- Add some features to AKS cluster

- Use some managed service

---
### Configuration(Before)

- Kubernetes Cluster(AKS)

  - Mattermost

  - Prometheus

  - Grafana

- Azure Load Balancer

- Azure Database for PostgreSQL server

---
### Configuration(After)

.zoom1[
- Kubernetes Cluster(AKS)

  - Mattermost

  - Prometheus

  - Grafana

  - <font color="DeepPink">Cert Manager</font>
  <br/>
  - <font color="DeepPink">Fluent Bit</font>

- Azure Load Balancer

- Azure Database for PostgreSQL server

- <font color="DeepPink">Azure Key Vault</font>
<br/>
- <font color="DeepPink">Azure Log Analytics</font>
]

---
class: center, middle, blue
# Demo

---
### Prerequisite

- (terraform) Create AKS cluster

---
### Step

1. (helm) Deploy ingress controller

2. (az) Set FQDN for public IP

3. (helm) Install cert manager

4. (kubectl) Deploy cluster issuer

5. (kubectl) Deploy flexvolume for Azure key vault

6. (kubectl) Deploy mattermost & ingress setting

7. (kubectl) Deploy prometheus & grafana & fluent bit

8. Grafana settings

---
### future prospects

.zoom1[
- ~~Secret data management~~

- ~~TLS support~~

- ~~Logging~~

  - ~~fluentd~~

- Continuous Delivery

  - Spinnaker/Tekton

- Service Mesh

  - Istio/SMI

- ~~Database~~ Azure services configuration management
]

---
class: center, middle, blue
# Thank you!
