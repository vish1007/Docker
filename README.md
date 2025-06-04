---

```markdown
# YT-MLOPS-Docker-Masterclass

This repository is part of my learning journey with Docker. The goal is to implement Docker using hands-on experiments, Docker Desktop, and Docker Hub, along with a simple Python project.

---

## 📁 Project Structure

```

.
├── app.py               # Simple Python script
├── bonus.txt            # Sample data file
├── dockerfile           # Dockerfile to build the container
├── requirements.txt     # Python dependencies
├── .gitignore
├── LICENSE
└── README.md

````

---

## 🚀 Docker Experiments

### ✅ 1. Build Docker Image

```bash
docker build -t docker-demo-app .
````

This builds a Docker image from your Dockerfile and tags it as `docker-demo-app`.

---

### ▶️ 2. Run the Docker Container

```bash
docker run -it docker-demo-app
```

Runs the image interactively inside a container.

---

### 📂 3. Run with Mounted Volume

```bash
docker run -it -v $(pwd):/app docker-demo-app
```

Mounts your local project directory inside the container.

---

## 🖥️ Docker Desktop

I used **Docker Desktop** to:

* Manage running containers and images via a GUI
* View logs and container stats
* Simplify Docker environment setup on my system

Docker Desktop made it easier to visualize what's happening inside containers without relying only on the terminal.

---

## ☁️ Docker Hub

I pushed my Docker image to Docker Hub:

### 🔐 Login

```bash
docker login
```

### 🏷️ Tag the Image

```bash
docker tag docker-demo-app vish1007/docker-demo-app:latest
```

### 📤 Push to Docker Hub

```bash
docker push vish1007/docker-demo-app:latest
```

You can view or pull the image from Docker Hub using:

```bash
docker pull vish1007/docker-demo-app:latest
```

👉 Visit: [https://hub.docker.com/u/vish1007](https://hub.docker.com/u/vish1007)

---

## 🎯 Learning Goals

* Learn Docker fundamentals
* Containerize a Python app
* Use Docker Desktop for management
* Publish images to Docker Hub
* Build confidence with real-world Docker workflows

---

## 🪪 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgment

Thanks to YouTube tutorials(Vikash Das), open-source guides, and the Docker community for helping me get started with containerization.
---
