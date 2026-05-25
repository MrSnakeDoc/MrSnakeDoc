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

## Network Architecture & Design Philosophy

I design infrastructure around **segmentation, explicit trust boundaries, and controlled exposure**.

Rather than relying on a flat network, workloads are isolated into dedicated zones based on function and risk level:

- infrastructure and virtualization  
- application services  
- edge ingress  
- development environments  
- untrusted and IoT devices  

External access is centralized through a dedicated edge layer acting as the only controlled ingress point between the internet and internal services.

The architecture follows a deny-by-default model with explicit firewall rules, reverse proxies, end-to-end TLS, and isolated internal networks.

The goal is not enterprise-scale complexity, but systems that are:

- predictable  
- maintainable  
- observable  
- secure by design  

This approach prioritizes operational clarity, reduced blast radius, and infrastructure that can evolve safely over time.

---

## Selected Projects

### 🔹 Navire *(ongoing)*  
Distributed notification orchestration platform written in Go.

- Core + dispatcher architecture  
- Transport-agnostic pub/sub layer (Redis Streams first)  
- Multi-channel adapters (Slack, Gotify, ntfy, Discord, more planned)  
- Observability-first design  

The project is currently in active development and remains private while the initial MVP stabilizes.

More details: https://github.com/mrsnakedoc/navire

> This repository is only an overview. The code is still private while in active development.

---

### 🔹 Homelab Blueprint  
Documented reference architecture for self-hosted infrastructure.

- Proxmox + Docker stack  
- Traefik ingress  
- Cloudflare tunnels  
- Monitoring & access control  

A practical example of how I structure and reason about infrastructure.

https://github.com/mrsnakedoc/homelab-blueprint

---

### 🔹 Keg  
CLI tool for **bootstrapping and maintaining local development environments** with **bulk package management**.

- Written in Go  
- Declarative YAML configuration
- Idempotent execution  
- Designed for fast workstation provisioning  

→ Focused on developer productivity and reproducibility.

https://github.com/mrsnakedoc/keg

---

### 🔹 Jump Blueprint  
Self-hosted service launcher using intelligent HTTP redirection.

- Browser address bar as infrastructure entry point  
- Fuzzy matching for internal services  
- Single source of truth via Homepage configuration  

Designed as an **architecture blueprint**, intended to be forked and adapted.

https://github.com/mrsnakedoc/jump-blueprint

---

### 🔹 Dotfiles Blueprint  
Opinionated, modular dotfiles focused on:

- reproducibility  
- maintainability  
- minimalism  

https://github.com/mrsnakedoc/dotfiles-blueprint

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
