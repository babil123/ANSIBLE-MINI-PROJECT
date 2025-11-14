# Ansible Web Server Automation — DevOps Mini Project

This project demonstrates how to use **Ansible** from **WSL** to configure and deploy a web server on an **AWS EC2 instance**.

## What this project does

✔ Installs Apache automatically  
✔ Starts and enables Apache service  
✔ Creates a custom directory on the server  
✔ Deploys a styled HTML webpage using **Ansible templates (Jinja2)**  
✔ Uses SSH key-based authentication  

## Project Structure

devops-mini-project/
├── inventory.ini
├── setup-webserver.yml
└── templates/
└── index.html.j2


## Commands to run

Ping the server:

```bash
ansible -i inventory.ini webserver -m ping

Deploy the web server:

ansible-playbook -i inventory.ini setup-webserver.yml



Technologies Used

- Ansible

- Apache HTTP Server

- AWS EC2

- WSL (Ubuntu)

- YAML / Jinja2



