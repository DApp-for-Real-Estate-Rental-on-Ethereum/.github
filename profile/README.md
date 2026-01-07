
# Decentralized Real Estate Rental dApp

A Microservices-Based, Blockchain-Powered Real Estate Rental Platform  
Built with **Ethereum, Spring Boot, Next.js, and DevOps Best Practices**

<div align="center">
  <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/projet_overview_finale.png" alt="Project Overview" width="100%" style="border-radius: 10px; margin: 30px 0;">
</div>

---

## Overview

This project presents a decentralized application (dApp) designed for **peer-to-peer real estate rentals**. By leveraging **Ethereum blockchain**, users can list, lease, and manage rental properties **without intermediaries**, ensuring transparent, secure, and trustless transactions.

The system adopts a **microservices architecture** powered by:

- **Spring Boot** for backend RESTful services  
- **Next.js (React)** for the frontend user interface  
- **Python** for AI-driven pricing suggestions
- **Hardhat + Solidity** for blockchain smart contracts  
- **AWS** for infrastructure  
- **Docker** for containerization  
- **CI/CD with Jenkins**, monitoring with **Prometheus + Grafana**

---

## Team & Roles

| | **Backend** | **Frontend** | **Cloud** | **DevOps & AI** | **Blockchain** |
|:---:|:---:|:---:|:---:|:---:|:---:|
| **Member** | **El Azzouzi Achraf** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/achraf.jpeg" width="100" height="100" style="object-fit:cover; border-radius:50%"> | **Essalhi Salma** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/salma.jpeg" width="100" height="100" style="object-fit:cover; border-radius:50%"> | **Kchibal Ismail** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/kchibal.jpeg" width="100" height="100" style="object-fit:cover; border-radius:50%"> | **El Gorrim Mohamed** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/mohamed.jpg" width="100" height="100" style="object-fit:cover; border-radius:50%"> | **Mohand Omar Moussa** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/moussa.jpeg" width="100" height="100" style="object-fit:cover; border-radius:50%"> |
| **Role** | Backend Engineer | Frontend Engineer | Cloud Engineer | DevOps & AI Engineer | Blockchain Engineer |
| **Description** | Spring Boot, REST APIs, DB Integration | Next.js Components, Web3 Integration, UX | AWS Infrastructure, Security, Storage | CI/CD Pipelines, Docker, Kubernetes, AI Pricing Models, Data Trends | Smart Contracts, Web3, Testnets |

---

## Architecture & CI/CD Pipelines

### AI/ML Pipeline

<div align="center">
  <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/documentations-reports/blob/main/LaTeX_format/images/ai_pipeline.png" alt="AI/ML CI/CD Pipeline" width="90%" style="border-radius: 10px; margin: 20px 0;">
</div>

**Jenkins CI/CD Pipeline for AI Pricing Services**

This pipeline automates the deployment of our **Python-based AI/ML pricing engine** that provides intelligent rent suggestions and market analysis:

- **Git Checkout**: Pulls the latest AI service code from the repository
- **Verify Layout**: Validates project structure and configuration files
- **Build & Test (pytest)**: Runs unit tests to ensure model accuracy and API reliability
- **Static Analysis (SonarQube)**: Performs code quality checks and identifies potential issues
- **Code Quality Validation**: Ensures code meets quality gates before deployment
- **Security Scan (Trivy)**: Scans for vulnerabilities in dependencies and Docker images
- **Model Validation**: Verifies ML model integrity and performance metrics
- **Build Docker Image**: Packages the AI service into a containerized image
- **Test Container**: Validates the Docker image runs correctly with health checks
- **Push to Docker Hub**: Publishes the verified image to the remote registry

The pipeline ensures that our AI models for **dynamic pricing**, **risk scoring**, **property recommendations**, and **market trends** are thoroughly tested and securely deployed.

---

### Backend Pipeline

<div align="center">
  <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/documentations-reports/blob/main/LaTeX_format/images/backend_pipeline.png" alt="Backend CI/CD Pipeline" width="90%" style="border-radius: 10px; margin: 20px 0;">
</div>

**Jenkins CI/CD Pipeline for Spring Boot Microservices**

This pipeline orchestrates the deployment of our **Java-based backend microservices** (API Gateway, User Service, Property Service, Booking Service, Payment Service, Notification Service, and Reclamation Service):

- **Git Checkout**: Retrieves the latest microservice code
- **Verify Layout**: Validates Maven project structure and dependencies
- **Build & Test (Maven)**: Compiles Java code and executes JUnit tests
- **Code Quality Check (SonarQube)**: Analyzes code quality, complexity, and test coverage
- **Publish Results (JUnit)**: Publishes test reports for review
- **Build JAR File**: Creates executable JAR packages for each microservice
- **Deploy to Docker**: Containerizes the microservices for deployment
- **Push to Docker Hub**: Uploads the images to the remote registry

The backend pipeline ensures that all microservices are built with consistent quality standards and ready for orchestration in our Kubernetes cluster.

---

### Frontend Pipeline

<div align="center">
  <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/documentations-reports/blob/main/LaTeX_format/images/frontend_pipeline.png" alt="Frontend CI/CD Pipeline" width="90%" style="border-radius: 10px; margin: 20px 0;">
</div>

**Jenkins CI/CD Pipeline for Next.js Application**

This pipeline manages the deployment of our **Next.js/React frontend** with Web3 integration:

- **Git Checkout**: Fetches the latest frontend code
- **Verify Layout**: Validates Node.js project structure and package.json
- **Install Dependencies (npm ci)**: Installs exact versions of dependencies for reproducibility
- **Linting (ESLint)**: Enforces code style and catches potential errors
- **Build App (next build)**: Compiles the Next.js application for production
- **Build Docker Image**: Creates a containerized version of the frontend
- **Push to Docker Hub**: Publishes the frontend image to the remote registry

The frontend pipeline ensures a seamless user experience with optimized builds, proper Web3 wallet integration (MetaMask), and responsive UI components.

---

### Cloud Architecture

<div align="center">
  <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/documentations-reports/blob/main/LaTeX_format/images/cloud_architecture.png" alt="Cloud Architecture" width="90%" style="border-radius: 10px; margin: 20px 0;">
</div>

**AWS Cloud-Native Infrastructure**

Our platform is deployed on **AWS** with a production-grade, highly available architecture:

#### **Network Layer**
- **VPC (10.0.0.0/16)**: Isolated virtual network with public and private subnets across multiple availability zones
- **CloudFront CDN**: Global content delivery for frontend assets, API endpoints, and blockchain RPC
- **Application Load Balancer (ALB)**: Distributes incoming traffic across microservices with health checks

#### **Compute & Orchestration**
- **Amazon EKS 1.30**: Managed Kubernetes cluster running all microservices
- **Worker Nodes (t3.medium)**: Auto-scaling node groups for optimal resource utilization
- **Workloads Pod**: Hosts all containerized services:
  - Frontend (Next.js)
  - API Gateway
  - Microservices (User, Property, Booking, Payment, Notification, Reclamation)
  - AI Pricing Engine
  - Blockchain Service
  - PostgreSQL Database
  - RabbitMQ Message Broker

#### **Storage & Registry**
- **Amazon ECR**: Private Docker image registry for all microservices
- **Amazon S3**: Object storage for property images, documents, and media uploads
- **Amazon RDS**: Managed PostgreSQL database for persistent data

#### **Security & DNS**
- **AWS Certificate Manager (ACM)**: SSL/TLS certificates for HTTPS encryption
- **Route 53**: DNS management and domain routing

#### **Monitoring & Observability**
- **Prometheus**: Metrics collection and time-series database
- **Grafana**: Visualization dashboards for system health and performance monitoring

This architecture ensures **scalability**, **high availability**, **security**, and **fault tolerance** for our decentralized real estate rental platform.

---

## Tech Stack

### Frontend
- **Next.js** (React Framework)
- TypeScript
- Tailwind CSS
- Leaflet.js (for interactive maps)  
- ethers.js / Web3.js  
- MetaMask  

### Backend
- **Spring Boot** (Java 17) - Core Microservices
- **Python** (v3.12) - AI Pricing Engine
- Maven
- JUnit / Pytest
- Web3j

### Blockchain
- Ethereum (Testnet)  
- Hardhat  
- Solidity
- Slither (smart contract static analysis)

### DevOps & Cloud
- **Docker & Docker Compose**
- **Jenkins** (CI/CD Pipelines)
- **Git LFS** (Model Storage)
- AWS (EC2, S3)
- Prometheus & Grafana (Monitoring)

## Architecture

The solution relies on a distributed system where the **API Gateway** orchestrates requests between the frontend and various specialized microservices (User, Property, Booking, Payment, Notification). The **AI Engine** provides real-time pricing intelligence, while the **Blockchain Service** ensures immutable, trustless lease agreements.
