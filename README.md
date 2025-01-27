# Alliedium DevOps course 2022

## 01 DevOps introductory and virtualization 20220809

- Virtualization: types, why to use
- Hypervisors: types, which to choose
- Proxmox: how does it work
- Demo: how to create a VM on Proxmox


## 02 Containers-1 20220811

- What is a Container
- Why did Containers appear
- Containers vs Virtual Machines
- How Containers are used
- Basic Concepts


## 03 Virtualization On Windows And ZFS 20220816

ZFS (Zettabyte file system)
- History, Advantages, Limitations
- Features: Pooled Storage, Copy-on-write, Snapshots


## 04a ZFS-2 20220818

ZFS Features
- Data integrity verification and automatic repair
- RAID handling
- Deduplication, Compression

Demo


## 04b Containers-2 20220818

- Some Tools (LXC, Docker, Kubernetes, Podman)


## 05 Docker Basic Commands 20220823

- Managing images and containres
- Demo: run PostgreSQL in a container, connect via psql from host

## 06 ProxMox2 SSH backup 20220825

- LVM Disk resize
- Setting access via SSH
- Backup and Restore

## 07 Docker Best Practices 1 20220830

- Dockerfile instructions
- Image parameterization
- Example 1: Simple Spring Boot application in a container with multi-stage build
- Example 2: pgAdmin in a container

## 08 Docker Best Practices 2 20220906

- Multistage builds
- Example 1: Simple Spring Boot application improved
- Example 2: Dockerfile of pytorch
- Example 3: Python dependences in a separate image parameterized by hash
- Example 4: CMD vs ENTRYPOINT
- Example 5: Isolation of containres by user-defined network
- Example 6: Put ca-certificates into base image, parameterize the image by certificates hash

## 09 Lvm Storage ssh Systemd cloudinit 20220908

- LVM extend with additional PV
- Alternative to resize2fs for XFS
- Different Storage Types
- systemd: how to create your own service
- Timers for fstrim
- SSH ciphers
- Cloud-Init
- Proxmox Command Line
- Ansible
- Terraform

## 10 Network part 1 20220913

- Hosts
- IP Address, Network, Repeater, Hub, Bridge, Switch, Router
- OSI and TCP/IP model
- How packets move through a network
- Protocols

## 11 Kubernetes development basic tools 20220915

Kubernetes deployment types
- in the cloud (EKS, AKS, GKE)
- prod-like on-prem / on bare metal (k0s, k3s, rke, rke2, kubespray, kubeadm, etc.)
- local (k3s, k3d, Kind, MicroK8S, Minikube, Docker Desktop, Rancher Desktop)

- Kubernetes development tools (k3d, kubectl + krew, vscode + plugin)
- Demo: managing clusters, contexts, namespaces. Running an app in a pod.

## 12 Network part 2 20220920

- Practice (nmtui, nmcli, arp, ip route)
- DNS (Root level domain, Top level domains, Second level domains, Recursive and Caching, Forwarding)
- TLS/SSL (what is, how protects data, CA)
- Hashing, Data integrity
- Encryption (asymmetric, symmetric; algorithms, public and private keys)
- How SSL/TLS uses Cryptography


## 13 Container orchestation Kubernetes basics 1 20220922

- Kubernetes development tools (code-server, k9s, openlens)
- Display Kubernetes current context in zsh command separator

## 14 Container orchestation Kubernetes basics 2 20220927

Deployment variants of Spring Boot Application with PostgerSQL database
- Example 1. Single pod with sidecar, ephemeral volume
- Example 2. Two pods, database in ephemeral volume

## 15 From network fundamentals to SDN implementation in Proxmox part 3 20220929

- Https, Certificates (DSA,CA, Cipher Suites, HSTS, SSL certificates)
- Demo: SSL termination with self-signed certificate

## 16 Network part 4 20221004

- Demo: SSL termination with self-signed certificate (ending)


## 17 Network part 4-1 20221006

- Demo: configure in opnsense plugin nginx for load balancing
- ACME protocol
- Demo: SSL termination with public certificate, using ACME and Route53


## 18 Container orchestation Kubernetes basics 3 20221011

Deployment variants of Spring Boot Application with PostgerSQL database
- Example 3. Added services and persistence via PVC
- Example 4. ReplicaSets, Readiness and Liveness probes

## 19 Container orchestration Kubernetes basics 4 20221013

Deployment variants of Spring Boot Application with PostgerSQL database
- Example 5. Deployment, StatefulSet, ConfigMap, Secret

Backup jobs configuration variants
- Example 6. Simple job with Minio S3 storage

## 20 Container orchestration Kubernetes basics 5 20221018

Backup jobs configuration variants
- Example 7a. CronJob with Localstack AWS S3 Bucket
- Example 7b. CronJob with real AWS S3 Bucket

Installing useful tools in Kubernetes
- Example 8. Installing pgAdmin

## 21 Container orchestration Kubernetes basics 6 20221020

Using aready existing Helm charts and operators
- Example 9. Installing PostgreSQL with metrics view via Grafana

## 22 VLANs with examples part 1 20221025

- Network virtualization, VLANs
- Example: Proxmox cluster with three VLANs for VMs and separate VLAN for proxmox nodes

## 23 VLANs with examples part 2 20221027

- Example: Proxmox cluster with three VLANs for VMs and separate VLAN for proxmox nodes (ending)
- SDN VLAN setup
- Cloud-init scripts

## 24 VLANs with examples part 3 20221101

- resolv.conf & netplan - correct network configuration setup on ubuntu
- Cloud-Init regenerate image & CLI
- SSH StrictHostKeyChecking
- Customize VMs via libguestfs-tools: virt-customize
- Example: Hyper-V with three VLANs for VMs and separate VLAN for proxmox nodes

## 25 Container orchestration Kubernetes basics 7 (beginning) 20221101

- Operators and Custom Resource Definitions
- Adding nodes to k3d cluster
- Step 1 of Example 10. Installing scalable PostgreSQL via Kubernetes operator

## 26 Container orchestration Kubernetes basics 7 20221103

- CRDs and Custom Resources
- PostgreSQL High Availability
- How to create a Helm Chart from manifests
- Steps from 2 to 7 of Example 10. Installing scalable PostgreSQL via Kubernetes operator
