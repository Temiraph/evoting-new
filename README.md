E-Voting Microservices Application

This project is a **cloud-native microservices-based e-voting system** built with containerized services and deployed on AWS EC2. It demonstrates best practices in **DevOps, CI/CD, and cloud deployment** using Docker, GitHub Actions, DockerHub, and Amazon ECR.

---

## 🚀 Architecture

The application consists of the following microservices:

- **Vote Service** – Handles user votes.
- **Result Service** – Displays voting results.
- **Worker Service** – Processes background jobs and updates results.
- **Redis** – Acts as a queue for handling vote processing.
- **PostgreSQL** – Stores voting data persistently.

All services are containerized with **Docker**, orchestrated using **Docker Compose**, and deployed on **AWS EC2**.  
Images are built and pushed automatically using **GitHub Actions** CI/CD pipeline to **DockerHub** and **Amazon ECR**.


## 🛠️ Tech Stack

- **Languages & Frameworks**: Python / Node.js   
- **Databases**: PostgreSQL, Redis  
- **Containerization**: Docker, Docker Compose  
- **CI/CD**: GitHub Actions → DockerHub + Amazon ECR  
- **Cloud Deployment**: AWS EC2  
- **Version Control**: Git + GitHub  

---

## ⚙️ Setup & Deployment

Clone the repository
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>

build and run locally (optional)
docker-compose up --build


This will start all microservices using local Dockerfiles.

CI/CD Pipeline

Each push triggers GitHub Actions.

GitHub Actions builds Docker images for each microservice.

Images are pushed to DockerHub and Amazon ECR.

Deployment on AWS EC2

SSH into your EC2 instance

Pull images from DockerHub:

docker-compose pull
docker-compose up -d


The application will be accessible at your EC2 public IP.
Architecture Diagram

Features

Fully containerized microservices architecture

CI/CD pipeline with GitHub Actions

Automated image builds and publishing

Deployment-ready on AWS EC2

Scalable and modular design
Contribution

Contributions are welcome! Feel free to fork the repo, submit issues, or open pull requests.
