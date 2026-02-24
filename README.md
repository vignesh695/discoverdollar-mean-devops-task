# MEAN Stack CRUD DevOps Deployment

This project demonstrates the deployment of a full-stack CRUD application using the MEAN stack (MongoDB, Express, Angular, Node.js) on AWS EC2 using Docker.

---

## 🚀 Deployment Steps

### 1️⃣ AWS EC2 Instance Created
- Instance Type: t3.micro
- Security Group Ports Opened:
  - 22 (SSH)
  - 80 (HTTP)
  - 8080 (Backend)

![EC2 Running](ec2-running.png)

---

### 2️⃣ SSH into EC2 Instance

```bash
ssh -i your-key.pem ubuntu@your-public-ip
```

---

### 3️⃣ Docker Installation

```bash
sudo apt update
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
```

---

### 4️⃣ Clone Repository

```bash
git clone https://github.com/vignesh695/discoverdollar-mean-devops-task.git
cd discoverdollar-mean-devops-task
```

---

### 5️⃣ Run Docker Compose

```bash
docker-compose up -d --build
```

---

### 6️⃣ Verify Running Containers

```bash
docker ps
```

![Docker Running](docker running.png)

---

## 🌐 Application Running on Browser

Access using:

```
http://100.53.115.27
```

![Tutorial List](Tutorial_list.png)

---

## ➕ CRUD Operations

### Add Tutorial
![Add](Tutorial_add.png)

### Submit Tutorial
![Submit](submit.png)

### View Tutorials
![List](Tutorial_list.png)

### Edit Tutorial
![Edit](Tutorial_edit.png)

### Remove All
![Remove](remove_all_button.png)

---

## 📂 GitHub Repository

![Repo](github_repo.png)

---

## ✅ Application Successfully Deployed on AWS EC2 using Docker
