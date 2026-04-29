# 📅 Day 6 – DevOps Challenge (Docker Basics & Networking)

## 🎯 Objective

Understand Docker fundamentals, run containers, and learn basic networking using port mapping.

---

## ⚙️ Environment Used

* Ubuntu (VMware)
* Docker Engine
* GitHub repository: `devops-challenge`

---

## 🐳 Introduction to Docker

* Docker is a containerization platform used to run applications in isolated environments
* Key concepts:

  * Image → Blueprint of application
  * Container → Running instance of image

---

## 🔧 Docker Installation & Setup

* Installed Docker using:

  * `sudo apt install docker.io -y`

* Started and enabled Docker service:

  * `sudo systemctl start docker`
  * `sudo systemctl enable docker`

* Added user to Docker group:

  * `sudo usermod -aG docker $USER`

* Applied changes using:

  * `newgrp docker`

---

## 🚀 Running Containers

### Basic Container Run

* Command:

  * `docker run nginx`

* Observation:

  * Container runs in foreground
  * Not accessible via browser

---

### Running Container in Background with Port Mapping

* Command:

  * `docker run -d -p 8080:80 nginx`

* Understanding:

  * `-d` → Run in background
  * `-p 8080:80` → Map host port 8080 to container port 80

---

## 🌐 Networking Concept (Important)

* Traffic flow:

  * Browser → localhost:8080 → Docker → Container:80

* Key terms:

  * localhost → your machine
  * Host port → 8080
  * Container port → 80

---

## 🔄 Container Management

### Stop container

* `docker stop <container_id>`

### Remove container

* `docker rm <container_id>`

---

## 🏷️ Named Container

* Created container with name:

  * `docker run -d -p 8080:80 --name Hari-Nginx nginx`

* Verified using:

  * `docker ps`

---

## 🛠 Docker Commands Practiced

* `docker ps` → list running containers
* `docker images` → list images
* `docker logs <container>` → view logs
* `docker exec -it <container> bash` → access container
* `docker restart <container>` → restart container

---

## 🔁 Port Mapping Change

* Learned that port mapping cannot be changed for running container
* To change port:

  * Stop container
  * Remove container
  * Re-run with new port

---

## 🧠 Key Learnings

* Docker containers are isolated runtime environments
* Port mapping is required to access container services
* Docker uses host-to-container networking
* Containers must be recreated to change configurations
* Permission issues can occur if user is not in docker group

---

## ✅ Outcome

* Successfully installed and configured Docker
* Ran Nginx container
* Accessed application via browser using port mapping
* Managed container lifecycle (start, stop, remove)
* Understood basic Docker networking

---

## 🚀 Next Step

Learn Dockerfile to build custom images and run your own applications (Day 7)
