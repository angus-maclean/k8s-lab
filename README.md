# k8s-prox-lab

Hardware:
Host - HP Prodesk 600 G3
Ram - 32GB
Hypervisor - Proxmox

Cluster Architecture:
k3s control - control plane - 2 cores - 4GB
k3s worker1  - worker - 2 cores - 8GB
k3s worker2 - worker - 2 cores - 8GB

Goal stack (working through this):
Kubernetes - k3s
Ingress - Traefik
Storage - Longhorn
Monitoring - Prometheus and Grafana
GitOps - ArgoCD

Also using: tmux and vim

Roadmap:
- install proxmox
- create VM templates
    - created Ubuntu Server 22.04 VM
    - installed qemu guest agent
    - disabled swap (required for kubernetes)
    - cleared machine-id for clean cloning
    - converted to proxmox template
    - cloned the template 3 times
    - applied static IP with netplan
    - changed correct hostnames with hostnamectl
- run k3s cluster
    - cluster running with 1 control node and 2 worker nodes.
    - give the worker nodes new labels
- configure ingress
- configure persistent storage with Longhorn
- Monitor the stack
- GitOps with ArgoCD
 
