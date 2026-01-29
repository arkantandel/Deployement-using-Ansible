<!-- BIG BANNER -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=220&section=header&text=Cloud%20Deployment%20Using%20Ansible&fontSize=45&fontColor=ffffff&animation=fadeIn" />
</p>

---

<h1 align="center">🚀 Automated Cloud Web Deployment</h1>
<h3 align="center">AWS EC2 + Ansible + Nginx + HTML Deployment</h3>

---

## 👨‍💻 Author

| Name | Role | Location |
|---|---|---|
| **Arkan Tandel** | DevOps Engineer (Fresher) | Pune, India |

📧 Email: arkantandel@gmail.com  
🔗 LinkedIn: https://linkedin.com/in/arkantandel  
🔗 GitHub: https://github.com/arkantandel  

---

## 🏷 Tech Stack Badges

![AWS](https://img.shields.io/badge/Cloud-AWS-orange?style=for-the-badge)
![Ansible](https://img.shields.io/badge/Automation-Ansible-red?style=for-the-badge)
![Linux](https://img.shields.io/badge/OS-Linux-yellow?style=for-the-badge)
![Nginx](https://img.shields.io/badge/WebServer-Nginx-green?style=for-the-badge)
![DevOps](https://img.shields.io/badge/Domain-DevOps-blue?style=for-the-badge)

---

# 🌟 Project Overview

This project demonstrates **Real World DevOps Cloud Automation** using:

✅ AWS EC2 Cloud Infrastructure  
✅ Ansible Configuration Management  
✅ Nginx Web Server Automation  
✅ HTML Website Deployment  



# 🏗️ Architecture Diagram

```mermaid
flowchart LR
    A[Developer Laptop] --> B[Ansible Control Node]
    B --> C[AWS EC2 Instance]
    C --> D[Nginx Web Server]
    D --> E[HTML Website]
    E --> F[User Browser]
```

---

# 📂 Project Structure

```mermaid
flowchart TD
    A[Project Root]
    A --> B[inventory.ini]
    A --> C[deploy.yml]
    A --> D[index.html]
```

---

# ⚙️ Installation Steps

---

## 🖥 Update System
```bash
sudo apt update -y
```

---

## ⚙ Install Ansible
```bash
sudo apt install ansible -y
```

---

# ☁ AWS EC2 Setup

Create Instance:

- Ubuntu Server  
- Open Port 22 (SSH)  
- Open Port 80 (HTTP)  

---

# 🔐 SSH Access

```bash
chmod 400 key.pem
ssh -i key.pem ubuntu@SERVER_IP
```

---

# 📄 Inventory Configuration

```ini
[production]
server1 ansible_host=YOUR_SERVER_IP ansible_user=ubuntu
```

---

# 📄 Deployment Playbook

```yaml
---
- name: Configure Nginx Web Server
  hosts: production
  become: yes

  tasks:

    - name: Install nginx
      apt:
        name: nginx
        state: latest
        update_cache: yes

    - name: Start nginx
      service:
        name: nginx
        state: started
        enabled: yes

    - name: Deploy Website
      copy:
        src: index.html
        dest: /var/www/html/index.html
```

---

# 📄 Website File

```html
<h1>🚀 Website Deployed Using Ansible</h1>
```

---

# 🚀 Deployment Command

```bash
ansible-playbook -i inventory.ini deploy.yml
```

---

# 🌐 Access Website

```
http://SERVER_IP
```

---

# 📚 DevOps Learning Path

```mermaid
flowchart LR
    A[Linux Basics] --> B[Networking]
    B --> C[AWS Cloud]
    C --> D[Ansible]
    D --> E[CI/CD]
    E --> F[Terraform]
```

---

# 🎯 Benefits

✅ Industry Level Automation Experience  
✅ Cloud Hands-on Experience  
✅ DevOps Real Workflow  
✅ Strong Resume Project  
✅ GitHub Portfolio Project  

---

# 🔥 Future Enhancements

- CI/CD Pipeline Integration  
- Docker Container Deployment  
- Terraform Infrastructure Automation  
- Multi Server Deployment  
- Ansible Roles Implementation  

---

# 💼 Resume Project Title

**Automated Cloud Web Deployment Using Ansible and AWS EC2**

---

# ❤️ DevOps Quote

> "Automation is not optional. It is survival in modern infrastructure."

---

<!-- FOOTER BANNER -->

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=120&section=footer"/>
</p>

