# 🚀 Strapi Docker Application

A containerized **Strapi CMS** application running locally using Docker.  
This project demonstrates how to run Strapi both **locally** and inside a **Docker container**, making it ready for cloud deployment and DevOps workflows.

---

## 📌 Tech Stack

- Strapi (Headless CMS)
- Node.js
- Docker
- SQLite (default local database)

---

Loom Video Walkthrough 🎥
Watch the full process in this Loom video:
🔗 https://www.loom.com/share/ba91f9ffa97a445ab7a685b7db7a7b7f

---

## 📁 Project Structure
.
├── config/
├── public/
├── src/
├── Dockerfile
├── .dockerignore
├── package.json
└── README.md

---

## ⚙️ Prerequisites

Make sure you have installed:

- Node.js (v18 recommended)
- npm
- Docker

Check versions:
  node -v
  npm -v
  docker -v

---

▶️ Run Strapi Locally (Without Docker)
1. Install dependencies
npm install

2. Start development server
npm run develop

3. Open in browser
  Admin Panel:
    http://localhost:1337/admin

---

🐳 Run Strapi Using Docker
1. Build Docker Image
    docker build -t strapi-local .

2. Run Docker Container
    docker run -p 1337:1337 --name strapi-container strapi-local

3. Access Application
  Admin Panel:
    http://localhost:1337/admin

📦 Docker Commands (Useful)
Run in background
docker run -d -p 1337:1337 --name strapi-container strapi-local

View logs
docker logs strapi-container

Stop container
docker stop strapi-container

Remove container
docker rm strapi-container

