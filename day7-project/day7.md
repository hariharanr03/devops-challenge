# 📅 Day 7 – DevOps Challenge (Dockerfile & Custom Image Basics)

## 🎯 Objective

Understand Dockerfile basics, image customization, and how Docker containers serve custom applications.

---

## ⚙️ Environment Used

* Ubuntu (VMware)
* Docker Engine
* Nginx Docker Image
* GitHub repository: `devops-challenge`

---

## 🐳 Dockerfile Introduction

* Learned that a Dockerfile is used to create custom Docker images
* Understood the workflow:

  * Dockerfile → Build Image → Run Container

---

## 🧠 Core Docker Concepts

### Image vs Container

* Image:

  * Blueprint/template of application

* Container:

  * Running instance of image

---

## 🔍 Understanding `FROM nginx`

### Dockerfile:

```dockerfile
FROM nginx
```

### Understanding:

* Uses official Nginx image as base image
* Does NOT install a full Linux operating system
* Docker containers share the host Linux kernel
* Nginx image already contains:

  * Minimal Linux layers
  * Nginx installed and configured

---

## 🖥️ Docker & Operating Systems

### Learned:

* Docker containers are based on Linux kernel features
* Docker works natively on Linux systems

### Windows/Mac Understanding:

* Docker Desktop internally runs a lightweight Linux VM
* Containers still depend on Linux kernel functionality

---

## 📄 Understanding `COPY`

### Dockerfile:

```dockerfile
COPY index.html /usr/share/nginx/html/index.html
```

### Understanding:

* Copies local `index.html` file into container
* Replaces default Nginx webpage

---

## 📂 Understanding Nginx Web Root

### Path Used:

```bash
/usr/share/nginx/html/
```

### Learned:

* This is the default web directory for Nginx
* Nginx serves webpages from this location

### How to Discover Such Paths:

* Read official documentation
* Explore inside container:

  * `docker run -it nginx bash`
  * `cd /usr/share/nginx/html`

---

## 🌐 Networking Understanding

### Request Flow:

Browser → localhost:8082 → Docker → Container:80 → Nginx → index.html

---

## 🧠 Key Learnings

* Docker containers are lightweight compared to VMs
* Docker uses host Linux kernel instead of full OS virtualization
* Base images already contain required software and minimal dependencies
* Dockerfile customizes existing images
* File paths inside containers can be explored manually or found in documentation

---

## ✅ Outcome

* Understood Dockerfile workflow
* Learned purpose of `FROM` and `COPY`
* Understood Linux kernel dependency in Docker
* Learned how Docker works across Windows, Mac, and Linux
* Understood how Nginx serves webpages inside containers

---

## 🚀 Next Step

Build custom Docker images and run personal applications using Dockerfile (Day 8)
