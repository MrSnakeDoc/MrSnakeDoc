<h1 align="center">
Platform & Infrastructure Engineer
</h1>

<h3 align="center">
Linux • Containers • Networking • Automation • Go
</h3>

<p align="center">
Building and operating reliable self-hosted systems — from homelab experimentation to production-oriented architectures.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Linux-✓-FCC624" />
  <img src="https://img.shields.io/badge/Docker-✓-2496ED" />
  <img src="https://img.shields.io/badge/Networking-✓-0A66C2" />
  <img src="https://img.shields.io/badge/Golang-✓-00ADD8" />
  <img src="https://img.shields.io/badge/Kubernetes-learning-326CE5" />
  <img src="https://img.shields.io/badge/Proxmox-✓-E57000" />
</p>

---

## About

Infrastructure & Platform Engineer with a strong **systems mindset**.

I focus on:

- Linux-based systems and containerized environments  
- Self-hosted infrastructure design and operations  
- Networking, reverse proxies, TLS, and access control  
- Automation and reproducibility  
- Writing small, focused tools in **Go** when automation requires it  

My background combines **development and operations**, with the goal of building platforms that are:

- understandable  
- observable  
- reproducible  
- easy to operate  

I use a real-world **homelab environment** as a continuous learning and experimentation platform to validate architectures before applying them in professional contexts.

---

## Infrastructure & Operations Experience

My homelab environment includes:

- **Virtualization**
  - Proxmox VE

- **Containers**
  - Docker & Docker Compose
  - Kubernetes (K3s – learning in progress)

- **Networking & Access**
  - Traefik reverse proxy
  - Automated TLS
  - Cloudflare Tunnels
  - Internal DNS & routing

- **Observability**
  - Prometheus
  - Grafana
  - Node exporter & container metrics

- **Core Services**
  - Gitea
  - Drone CI
  - Authentik
  - Uptime Kuma
  - Gotify
  - Homepage
  - Mealie
  - Outline

- **Storage & Backup**
  - Synology NAS
  - Local backups & service persistence

This environment is intentionally treated as **infrastructure**, not a demo lab:
changes are versioned, documented, and reproducible.

---

## Network Architecture & Design Philosophy

I design network architectures with a strong focus on **segmentation, explicit trust boundaries, and controlled exposure**.

Rather than operating a flat network, my infrastructure is intentionally structured around multiple isolated zones, each with a clearly defined responsibility:

- infrastructure (virtualization, storage)  
- application workloads  
- edge exposure  
- development environments  
- untrusted devices  

Each workload is placed in its own network segment based on **risk level and function**, not convenience.  
This approach allows failures, misconfigurations, or compromises to remain contained by design.

External access is never granted directly to internal services.

All inbound traffic is funneled through a dedicated **edge layer**, acting as a strict choke point between the internet and internal networks.  
The edge has no implicit trust and is only allowed to forward explicitly defined traffic to the application layer, preventing lateral exposure.

Service access follows a layered model:

- DNS is treated as a first-class infrastructure component  
- reverse proxies act as clear trust boundaries  
- TLS is enforced end-to-end  
- internal networks remain non-routable from the internet  

Internal services are reachable only through authenticated reverse proxy paths or private access channels, never via direct IP exposure.

This architecture prioritizes:

- predictable traffic flows  
- reduced blast radius  
- minimal attack surface  
- operational clarity  

The goal is not enterprise-scale complexity, but **systems that are easy to reason about, secure by design, and safe to evolve over time**.

This approach does not aim to be an impenetrable fortress, but a pragmatic and continuously evolving system built around clear boundaries, explicit assumptions, and conscious trade-offs.

---

## Selected Projects

### 🔹 Navire *(ongoing)*  
Distributed notification orchestration platform written in Go.

- Core + dispatcher architecture  
- Transport-agnostic pub/sub layer (Redis Streams first)  
- Multi-channel adapters (Slack, Gotify, ntfy, Discord, more planned)  
- Observability-first design  

The project will be open-sourced once the initial MVP is stable but you can read more about it here:
https://github.com/mrSnakedoc/navire

> This repository is only an overview. The code is still private while in active development.

---

### 🔹 Homelab Blueprint  
Documented reference architecture for self-hosted infrastructure.

- Proxmox + Docker stack  
- Traefik ingress  
- Cloudflare tunnels  
- Monitoring & access control  

A practical example of how I structure and reason about infrastructure.

https://github.com/MrSnakeDoc/homelab-blueprint

---

### 🔹 Keg  
CLI tool for **bootstrapping and maintaining local development environments** with **bulk package management**.

- Written in Go  
- Declarative YAML configuration
- Idempotent execution  
- Designed for fast workstation provisioning  

→ Focused on developer productivity and reproducibility.

https://github.com/MrSnakeDoc/keg

---

### 🔹 Jump Blueprint  
Self-hosted service launcher using intelligent HTTP redirection.

- Browser address bar as infrastructure entry point  
- Fuzzy matching for internal services  
- Single source of truth via Homepage configuration  

Designed as an **architecture blueprint**, intended to be forked and adapted.

https://github.com/MrSnakeDoc/jump-blueprint

---

### 🔹 Dotfiles Blueprint  
Opinionated, modular dotfiles focused on:

- reproducibility  
- maintainability  
- minimalism  

https://github.com/MrSnakeDoc/dotfiles-blueprint

---

### 🔹 Goslaw  
Small Go library providing functional helpers for slice operations. Not a real lib ready for production use, but useful for learning Go generics.

https://github.com/MrSnakeDoc/goslaw

---

## Interests & Focus Areas

- Platform engineering  
- Infrastructure automation  
- Linux systems  
- Networking fundamentals  
- Container orchestration  
- Internal tooling  
- Developer experience  
- Reliability over novelty  

---

## Contact

- 📧 **Email**: dev@nexacloud.dev  
- 💼 **LinkedIn**: https://www.linkedin.com/in/sami-etech

---

> I am not focused on building trendy products.  
> I focus on building systems that are understandable, operable, and durable.
