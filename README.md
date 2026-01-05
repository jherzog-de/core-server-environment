# Docker Compose Stack: Traefik & Portainer

This repository provides a **Docker Compose stack** consisting of **Traefik** as a reverse proxy and **Portainer** for Docker container management.

Traefik is responsible for:
- automatic service routing
- **automatic SSL certificate generation via Let's Encrypt**
- securing the Traefik dashboard using Basic Authentication

---

## 🧩 Included Components

- **Traefik**
  - Reverse proxy
  - Automatic HTTPS certificates via Let's Encrypt
  - Web dashboard (protected by authentication)
- **Portainer**
  - Web-based Docker management
  - Accessed securely via Traefik and HTTPS

---

## 📁 Project Structure

```text
.
├── docker-compose.yml
├── .env
├── access.sh
└── traefik
    ├── traefik.yml
    └── secrets
        └── dashboard.htpasswd
```

---

## ⚙️ Required Configuration

Before starting the stack, you must adjust the **.env** file and run (or adapt) the access.sh script. 