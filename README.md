# 🚀 Containerizing vProfile with Docker Compose

This project demonstrates how to containerize a multi-tier Java web application (vProfile) using Docker and Docker Compose.

It covers how to:

- Analyse an application stack  
- Write Dockerfiles from scratch  
- Use official Docker images  
- Wire multiple services using Docker Compose  
- Deploy a full working system (Web + App + DB + Cache + Broker)  

---

# 🧠 Project Overview

vProfile is a multi-tier Java application consisting of:

- **Nginx (Web Server)** → Reverse proxy  
- **Tomcat (App Server)** → Runs Java application  
- **MySQL (Database)** → Stores user data  
- **Memcached (Cache)** → Improves performance  
- **RabbitMQ (Message Broker)** → Async communication  

---

# 🔁 Flow of Request

Browser → Nginx → Tomcat → MySQL / Memcached / RabbitMQ  

---

# 📁 Project Structure

vprofile-project/
├── src/
├── pom.xml
├── docker-compose.yml
├── docker-files/
│   ├── app/
│   │   └── Dockerfile
│   ├── db/
│   │   ├── Dockerfile
│   │   └── db_backup.sql
│   └── web/
│       ├── Dockerfile
│       └── vprofile.conf

##Images
![docker-compose-images](

Author

Built by **Seeqgold** as part of a DevOps learning journey
