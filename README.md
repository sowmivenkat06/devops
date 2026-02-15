# DevOps Practical Learning – 6 Day Journey

## 🎯 Aim
To understand and practice foundational DevOps tools and workflows including:
- Linux basics
- Version control with Git & GitHub
- Containerization with Docker
- CI/CD automation using Jenkins
- Cloud deployment with AWS
- Infrastructure automation with Ansible and Terraform

This documentation outlines the outcomes and procedures followed over six days of practical DevOps learning.

---

## 🛠️ Procedure

### 📅 Day 1 – Linux Fundamentals, VM & Basic Commands
- Learned differences between Windows and Linux operating systems.
- Explored Virtual Machines (VM) and Ubuntu installation via VMware.
- Understood Windows Subsystem for Linux (WSL) advantages.
- Practiced basic Linux commands: `pwd`, `ls`, `cd`, `mkdir`, `touch`, `cp`, `mv`, `rm`, `cat`, `grep`, `chmod`.
- Package management using APT: `sudo apt update`, `sudo apt upgrade`, `sudo apt install`.
- Learned use of Vi editor and LTS concepts.

---

### 🐳 Day 2 – Docker & Git Implementation
- Studied IPv4 address allocation and static vs dynamic IP assignment.
- Gained overview of Docker: containers, images, Dockerfiles.
- Built and ran a sample Node.js Docker application.
- Practiced Docker commands: build image, run containers, expose ports.
- Worked with DockerHub: login, tag, push, pull images.
- Setup Git & GitHub: initialize repo, commit, remote link, push commits.
- Solved a merge conflict issue while pushing to GitHub.

---

### 🔁 Day 3 – Docker Push, GitHub & Introduction to Jenkins
- Pushed Docker images to Docker Hub.
- Executed Git push operations from Ubuntu.
- Explored Git basics: commits, branches, history (`git log`), resolving conflicts.
- Introduced Jenkins for CI/CD.
- Installed Jenkins & Java; explained Jenkins use in automated build and deployment.
- Learned Git workflows and team collaboration basics.

---

### ⚙️ Day 4 – Jenkins Setup and CI/CD Pipeline
- Installed Jenkins on Ubuntu via repository and key setup.
- Started Jenkins service and accessed dashboard via web.
- Created Jenkins jobs (Freestyle projects) with build triggers.
- Explained upstream & downstream jobs in CI workflows.
- Defined pipeline structure for Git → Jenkins → Docker build flow.
- Installed key Jenkins plugins: Git, Docker Pipeline.
- Learned scripted pipeline stages: clone, install dependencies, build.
- Covered Jenkins triggers: manual, webhooks, cron scheduling.

---

### ☁️ Day 5 – AWS EC2 Deployment
- Created AWS EC2 instances (Ubuntu & Windows) with key pairs.
- SSH connected to Ubuntu EC2 instance.
- Installed Apache server and tested default web page.
- Deployed a sample HTML & GitHub project to Apache.
- Connected to Windows server via RDP.
- Learned to manage EC2 instances and avoid unnecessary billing.

---

### 🔧 Day 6 – DevOps Automation, Ansible & Terraform
- Documented standard DevOps lifecycle: GitHub → Jenkins → Infrastructure → Configuration.
- Configured Jenkins to pull code using GitHub credentials.
- Created Freestyle Jenkins jobs with basic build steps.
- Introduced Ansible for configuration management:
  - Installed Ansible, created inventory, verified SSH connectivity.
  - Wrote a playbook to install Nginx.
- Explained Terraform workflow: `init`, `validate`, `plan`, `apply`, `destroy`.
- Covered infrastructure as code fundamentals and Terraform commands.
- Discussed Master–Slave architecture, roles, benefits, and challenges.

---

## 📝 Conclusion
Over six days of practical exercises, this DevOps training covered key tools and workflows required for modern software development and operations:

✔ Strong command over Linux fundamentals  
✔ Building and managing Docker containers  
✔ Source control with Git & GitHub  
✔ Continuous integration & deployment using Jenkins  
✔ Cloud deployment on AWS EC2  
✔ Automation with Ansible  
✔ Infrastructure provisioning with Terraform  

Each day built upon the last to form a comprehensive DevOps skill set that enables automated build, test, and deployment pipelines, scalable infrastructure management, and efficient collaboration.
