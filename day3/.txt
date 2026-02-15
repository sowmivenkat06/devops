🐳 Docker – Push & GitHub Push (Ubuntu Commands)
Docker Hub Login
sudo docker login

Tag Image
docker tag ecommerce-app sowmiya2t/ecommerce:latest

Push to Docker Hub
docker push sowmiya2t/ecommerce:latest

🔧 Git Push to GitHub
Initialize Git
git init

Add Files
git add .

Commit
git commit -m "New e-commerce project"

Add Remote Repository
git remote add origin https://github.com/sowmivenkat06/devops.git

Push to GitHub
git branch -M main
git push -u origin main

🖥 VMware Ubuntu – System & Network Checks
more /etc/os-release        # Check Ubuntu version
ifconfig                    # Show network details
ip addr                     # Show IP address
ping -c 3 google.com        # Check internet connectivity

📘 Git – Basic Explanation
What is Git?

Git is a version control system used to track changes in source code.
It helps manage project history and collaboration.

Main Branch

Default branch of repository

Usually called main

Contains stable code

Feature Branch

Created from main branch

Used for new features or bug fixes

Later merged into main

Example:

main → feature-login → merge → main

🔄 Git Workflow (Ubuntu → GitHub)
1️⃣ Create Project Folder
mkdir myproject
cd myproject

2️⃣ Initialize Git
git init

3️⃣ Create Files

Create file:

touch file.txt


Overwrite file:

echo "Hello World" > file.txt


Append content:

echo "Second line" >> file.txt


> → Overwrite

>> → Append

4️⃣ Add Files
git add .

5️⃣ Commit Changes
git commit -m "Added file"

6️⃣ Connect to GitHub
git remote add origin https://github.com/sowmivenkat06/devops.git

7️⃣ Push to GitHub
git push -u origin main

📌 Git Concepts
Append / Insert in Git

When modifying a file:

git add .
git commit -m "Updated file"
git push

Git History

View commit history:

git log


Each commit has a unique hash ID.

HEAD & Tail

HEAD → Points to latest commit

Tail → First (oldest) commit

Example:

Tail ---- Commit1 ---- Commit2 ---- HEAD

⚠️ Merge Conflict Faced
Problem

While pushing code:

GitHub already had a README.md

Local project had different history

Error:

failed to push some refs

Solution
Step 1
git pull origin main --allow-unrelated-histories

Step 2

Edited conflicting sections

Saved README.md

Step 3
git add .
git commit -m "Resolved merge conflict"

Step 4
git push origin main

🐳 Docker – CI/CD Flow

Project Uses:

Ubuntu

GitHub

Node.js

Docker

Jenkins

Flow:

Developer → GitHub → Jenkins → Docker Build → Docker Run → Application Live

🔧 Jenkins
What is Jenkins?

Jenkins is an open-source automation tool used for:

Continuous Integration (CI)

Continuous Deployment (CD)

It automatically:

Builds code

Tests code

Deploys applications

Why Jenkins?

Automates manual work

Saves time

Reduces errors

Ensures continuous deployment

⚙️ Jenkins Installation (Ubuntu 24.04)
1️⃣ Install Java (Required)
sudo apt update
sudo apt upgrade
sudo apt install openjdk-21-jdk
java --version

2️⃣ Install Jenkins
sudo apt install jenkins
systemctl status jenkins

3️⃣ Customize Jenkins (Optional)

Stop Jenkins:

sudo systemctl stop jenkins


Edit configuration:

sudo systemctl edit jenkins


Restart:

sudo systemctl start jenkins

4️⃣ Fix Directory Permissions
sudo chown -R jenkins:jenkins /path

5️⃣ Check Logs
journalctl -u jenkins

6️⃣ Access Jenkins Web UI

Open:

http://your-server-ip:8080


Get password:

/var/lib/jenkins/secrets/initialAdminPassword


Then:

Install suggested plugins

Create admin user

Start using Jenkins
