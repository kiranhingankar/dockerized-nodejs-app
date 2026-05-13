# Dockerized Node.js App

## Overview
A simple Node.js + Express + MongoDB application fully containerized using Docker and Docker Compose.

---

## Features
- Multi-stage Docker build
- Non-root container
- MongoDB integration
- Persistent volumes
- Environment variable support
- Healthchecks

---

## Run the App

### Clone Repository

git clone <repo-url>

### Start Containers

docker compose up --build

### Stop Containers

docker compose down

---

## Environment Variables

PORT=3000
MONGO_URI=mongodb://mongo:27017/devopsdb

---

## Docker Hub Image

docker pull khingankar/dockerized-nodejs-app:tagname
