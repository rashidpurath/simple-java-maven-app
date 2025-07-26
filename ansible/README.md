# 🚀 Ansible Project: Automate Node.js App Deployment

This project demonstrates how to use Ansible to automate the provisioning and deployment of a Node.js application on a remote server.

## 🔧 Tools Used
- Ansible
- DigitalOcean / AWS EC2
- Node.js & npm
- Linux (Ubuntu)
- SSH Keys

## 📁 Project Structure
- `inventory/hosts.ini` - defines managed servers
- `playbooks/install_node.yml` - installs Node.js and npm
- `playbooks/deploy_app.yml` - deploys and starts the app
- `playbooks/create_user.yml` - creates a Linux user for the app

## ▶️ How to Run

```bash
ansible-playbook -i inventory/hosts.ini playbooks/install_node.yml
ansible-playbook -i inventory/hosts.ini playbooks/create_user.yml
ansible-playbook -i inventory/hosts.ini playbooks/deploy_app.yml

