# 🐳 Docker Task Manager

A simple **Dockerized microservices task manager application** built using **Flask, MongoDB, and Nginx**.
This project demonstrates how multiple services run together using **Docker Compose** to create a containerized web application.

---

# 📌 Project Overview

This project is a **task management web application** where users can:

* Add tasks
* View tasks
* Delete tasks
* Store tasks in a database

The entire application runs inside **Docker containers**, showcasing a **microservices architecture** commonly used in modern DevOps environments.

---

# 🛠 Tech Stack

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Python Flask
* **Database:** MongoDB
* **Containerization:** Docker
* **Orchestration:** Docker Compose
* **Web Server:** Nginx

---

# 🏗 Architecture

Browser
⬇
Nginx (Frontend Container)
⬇
Flask API (Backend Container)
⬇
MongoDB (Database Container)

All services communicate through the **Docker network created by Docker Compose**.

---

# 📂 Project Structure

docker-task-manager
│
├── frontend
│   └── index.html
│
├── backend
│   ├── app.py
│   ├── requirements.txt
│   └── Dockerfile
│
└── docker-compose.yml

---

# 🚀 How to Run the Project

### 1️⃣ Clone the repository

git clone https://github.com/YOUR_USERNAME/docker-task-manager.git

### 2️⃣ Navigate to the project folder

cd docker-task-manager

### 3️⃣ Run the application

docker compose up --build

---

# 🌐 Access the Application

Once the containers start, open your browser and visit:

http://localhost:8080

You will see the **Docker Task Manager dashboard**.

---

# 🐳 Docker Services

The project runs three containers:

• **Frontend Container**

* Built using Nginx
* Serves the static HTML dashboard

• **Backend Container**

* Python Flask REST API
* Handles task creation and deletion

• **Database Container**

* MongoDB database
* Stores tasks persistently

---

# 📡 API Endpoints

GET /tasks
Returns the list of tasks

POST /tasks
Adds a new task

DELETE /tasks/{task}
Deletes a specific task

---

# 💡 Key Concepts Demonstrated

* Docker containerization
* Multi-container applications
* Docker Compose orchestration
* REST API development
* Container networking
* Persistent database storage

---

# 🎯 Learning Outcome

This project demonstrates how to:

* Containerize applications using Docker
* Run multiple services with Docker Compose
* Connect frontend, backend, and database services
* Build a simple microservices architecture
