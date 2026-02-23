# Fullstack Monorepo Template 🚀

This repository is a starting template for building and deploying a fullstack web application. It uses a **monorepo** architecture, keeping both the frontend and backend in a single repository to ensure version synchronization and simplify the CI/CD pipeline.

## 🛠️ Tech Stack
* **Backend:** Java 21 (Spring Boot)
* **Frontend:** React (Bootstrapped with Vite)
* **Database:** PostgreSQL (Configured for Docker)
* **CI/CD:** Jenkins (Automated build & deployment)

## 📁 Repository Structure
```text
/
├── backend/               # Java 21 API (Spring Boot)
├── frontend/              # React User Interface
├── Jenkinsfile            # Pipeline configuration for Jenkins CI/CD
└── README.md