# 🛡️ Ansible Linux Hardening Tool

Automated security hardening for Debian/Ubuntu servers. This playbook implements industry best practices to protect your infrastructure from common attacks.

## ✨ Features
- **SSH Hardening:** Disables root login, changes default port, and enforces SSH key authentication.
- **Firewall Setup:** Configures `UFW` to deny all incoming traffic except essential ports.
- **Brute-force Protection:** Installs and configures `Fail2Ban`.
- **Auto-Updates:** Enables `unattended-upgrades` for critical security patches.
- **System Audit:** Updates all system packages to the latest secure versions.

## 🚀 How to use
1. Install Ansible: `pip install ansible`
2. Edit `inventory.ini` with your server IP.
3. Run the playbook:
   ```bash
   ansible-playbook -i inventory.ini playbook.yml
