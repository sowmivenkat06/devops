# 🚀 DevOps Project – Docker & Git Implementation

---

# 🌐 IPv4 – Address Allocation

IPv4 is a **32-bit addressing system** used to identify devices in a network.  
Format: `192.168.1.10` (four numbers separated by dots, range 0–255)

## Types of IP Assignment

### 1️⃣ Static IP (Manual)
- Assigned manually by administrator
- Does not change
- Used for servers, printers

### 2️⃣ Dynamic IP (Automatic)
- Assigned automatically using DHCP
- Changes when device reconnects
- Used for laptops and mobile devices

### Purpose
Ensures every device has a **unique IP address** for communication.

---

# 🐳 Docker Overview

Docker is a container platform used to run applications in isolated environments called **containers**.

A container includes:
- Application code
- Required libraries
- Runtime
- Configuration files

## Why Docker?
- ✅ Portability – Runs anywhere
- ✅ Lightweight – Faster than Virtual Machines
- ✅ Consistency – Same environment in dev, test, production

---

## Important Docker Terms

| Term        | Description |
|------------|------------|
| Image       | Blueprint of the application |
| Container   | Running instance of image |
| Dockerfile  | File used to build Docker image |

---

# 📦 Project 1: docker_sample (Node.js App)

## Application Code (app.js)

```js
const express = require('express');
const app = express();

app.get('/', (req, res) => {
  res.send('Hello from Docker!');
});

app.listen(3000, '0.0.0.0', () => {
  console.log('App running on port 3000');
});

# 📦 Project 1: Docker Sample (Node.js Application)

## 🔹 Application Explanation

- **express** → Web framework for Node.js  
- **app.get('/')** → Defines homepage route  
- **res.send()** → Sends response to browser  
- **app.listen(3000)** → Runs server on port 3000  
- **'0.0.0.0'** → Makes application accessible outside the container  

---

## 🐳 Dockerfile

```dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD ["node", "app.js"]

🐳 Docker Commands
Build Image
docker build -t docker-sample .

Run Container
docker run -d -p 3000:3000 --name docker_sample_app docker-sample

Access Application
http://localhost:3000


or

http://192.168.136.128:3000

📦 Project 2: day3/e-commerce (Dockerized Application)
Build Image
docker build -t ecommerce-app .

Run Container
docker run -d -p 8080:80 ecommerce-app

Open in Browser
http://localhost:8080

🐳 Docker Hub Operations
Login
docker login

Tag Image
docker tag ecommerce-app sowmiya2t/ecommerce:latest

Push Image
docker push sowmiya2t/ecommerce:latest

Pull Image (Other System)
docker pull sowmiya2t/ecommerce:latest

🔧 Git & GitHub Setup
Initialize Git
git init

Add Files
git add .

Commit
git commit -m "Initial commit"

Connect to GitHub Repository
git remote add origin git@github.com:sowmivenkat06/devops.git

Push to GitHub
git branch -M main
git push -u origin main

⚠️ Merge Conflict Faced
Issue

While pushing to GitHub, a merge conflict occurred because:

GitHub repository already had a README.md

Local project had a different commit history

Error
failed to push some refs

Solution
Step 1: Pull Remote Changes
git pull origin main --allow-unrelated-histories

Step 2: Resolve Conflict

Edited conflicting sections in README.md

Saved the file

Step 3: Commit Changes
git add .
git commit -m "Resolved merge conflict"

Step 4: Push Again
git push origin main

📜 Clean Command History (Filtered)
whoami
sudo apt update
sudo apt upgrade -y
sudo apt install docker-ce docker-ce-cli containerd.io
docker --version
git clone https://github.com/jagadeeshkanna97/docker_sample
cd docker_sample
docker build -t docker-sample .
docker run -d -p 3000:3000 docker-sample
ip a
ssh sowmiya@192.168.136.128
git init
git add .
git commit -m "Initial commit"
git remote add origin git@github.com:sowmivenkat06/devops.git
git push -u origin main




