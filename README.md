# 📝 Django Notes App

A full-stack, containerized notes management application with a **Django REST Framework backend**, **React.js frontend**, and **MySQL database**, deployed behind **Nginx** using **Docker & Docker Compose**.

---

## 🚀 Tech Stack

* **Backend:** Django REST Framework (REST API)
* **Frontend:** React.js
* **Database:** MySQL 8.0
* **Web Server:** Nginx (Reverse Proxy)
* **Containerization:** Docker & Docker Compose
* **Version Control:** Git

---

## 📦 Requirements

Ensure you have the following installed before running the app:

* **Python** 3.9
* **Node.js** (Latest LTS recommended)
* **React.js**

---

## ⚙️ Installation & Setup

### **1️⃣ Clone the Repository**

```bash
git clone https://github.com/fqabdullah/Django-NGNIX-deploy_web.git
cd django-notes-app
```

---

### **2️⃣ Environment Variables**

Create a `.env` file in the project root:

```env
DB_NAME=test_db
DB_USER=root
DB_PASSWORD=root
DB_PORT=3306
DB_HOST=db_cont
```

---

### **3️⃣ Run with Docker Compose**

```bash
docker compose up --build
```

---

### **4️⃣ Run Manually (Without Compose)**

**Build the image:**

```bash
docker build -t notes-app .
```

**Run the container:**

```bash
docker run -d -p 8000:8000 notes-app:latest
```

---

## 🌐 Nginx Reverse Proxy Setup

**Install Nginx:**

```bash
sudo apt-get update
sudo apt install nginx
```
