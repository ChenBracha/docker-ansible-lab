# 🐳 Docker-Ansible Lab

Spin up a mini-lab with one **Ansible Controller** and four **SSH-enabled nodes** (`web1`, `web2`, `db1`, `db2`)—all in Docker.  
Perfect for practicing playbooks, testing roles, or demoing Ansible concepts—no need for real servers, SSH keys, or `id_rsa`.

---

## ✨ Features
- **Controller + 4 Nodes** all networked together with Docker  
- Ready-to-use **password login** (`ansible` / `ansible`)  
- **No SSH keys needed**—authentication is via simple username & password  
- Minimal example **playbook.yml**: ping all hosts

---

## 🗺️ Directory Layout
*(everything is in the project root—no sub-folders)*

```text
.
├── Dockerfile.controller   # Docker image for the Ansible controller
├── Dockerfile.node         # Docker image used for all nodes
├── docker-compose.yml      # Spins up the full lab
├── ansible.cfg             # Ansible configuration
├── hosts.ini               # Ansible inventory (lists all nodes)
├── playbook.yml            # Sample playbook with basic tasks
└── README.md               # This file
