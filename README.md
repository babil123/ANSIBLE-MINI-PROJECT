# Ansible Web-Server Automation 🛠️

![Ansible](https://img.shields.io/badge/Ansible-2.14-blue?style=flat&logo=ansible)  
![AWS](https://img.shields.io/badge/AWS-EC2-orange?style=flat&logo=amazon-aws)  
![Apache](https://img.shields.io/badge/Apache-HTTP-Server-red?style=flat&logo=apache)  
![GitHub Actions](https://img.shields.io/badge/CI-GitHub_Actions-purple?style=flat&logo=github)  

## 🎯 Project Overview

This is a **DevOps mini-project** built to demonstrate how to automate deployment of a web server using:  
- Ansible (on WSL/Ubuntu)  
- AWS EC2 instance  
- Apache HTTP server  
- A styled HTML page deployed via Jinja2 template  

👉 You can view the live demo at: `http://100.28.122.5/demo/`

---

## 🧭 Architecture

WSL Ubuntu ── Ansible ──┐
SSH
[AWS EC2] ── Apache HTTP Server ── Demo Web Page


---

## 🗂️ Project Structure

ansible-mini-project/
├── inventory.ini
├── setup-webserver.yml
├── templates/
│ └── index.html.j2
└── README.md


---

## ✅ What This Project Does

- Installs Apache automatically via Ansible  
- Starts and enables the Apache service  
- Creates a dedicated directory (`/var/www/html/demo/`)  
- Deploys a styled HTML webpage using a Jinja2 template  
- Demonstrates end-to-end automation from your local machine (WSL) to AWS  

---

## 🚀 How to Run It

1. Edit `inventory.ini`, replacing `<YOUR_EC2_PUBLIC_IP>` and `/path/to/your/key.pem`  
2. On WSL Ubuntu, run:
   ```bash
   ansible -i inventory.ini webserver -m ping
   ansible-playbook -i inventory.ini setup-webserver.yml

![devops-mini](https://github.com/user-attachments/assets/b34f5ad0-3d83-4916-9436-83749d178de4)


🔧 Technologies Used

Ansible – configuration & orchestration

AWS EC2 – cloud compute

Apache HTTP Server – web server

WSL (Ubuntu) – development environment on Windows

YAML & Jinja2 – automation scripts & templating

📈 Future Improvements

Containerize the web server with Docker

Use Ansible to install and run Docker

Build CI/CD pipeline with GitHub Actions

Use Terraform to provision AWS infrastructure automatically

Add monitoring (Prometheus + Grafana) to the EC2 instance

Use secure secrets management for SSH keys

📬 Contact & License

Built by Babil — feel free to clone, fork, and extend.
This project is licensed under the MIT License
.

