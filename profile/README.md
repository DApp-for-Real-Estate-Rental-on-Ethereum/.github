
# Decentralized Real Estate Rental dApp

A Microservices-Based, Blockchain-Powered Real Estate Rental Platform  
Built with **Ethereum, Spring Boot, Next.js, and DevOps Best Practices**

<div align="center">
  <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/projet_overview.png" alt="Project Overview" width="100%" style="border-radius: 10px; margin-bottom: 20px;">
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

| | **Backend** | **Frontend** | **Blockchain** | **DevOps / AI & Data** | **Cloud** |
|:---:|:---:|:---:|:---:|:---:|:---:|
| **Member** | **El Azzouzi Achraf** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/achraf.jpeg" width="100" height="100" style="object-fit:cover; border-radius:50%"> | **Essalhi <br> Salma** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/salma.jpeg" width="100" height="100" style="object-fit:cover; border-radius:50%"> | **Mohand Omar Moussa** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/moussa.jpeg" width="100" height="100" style="object-fit:cover; border-radius:50%"> | **El Gorrim <br> Mohamed** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/mohamed.jpg" width="100" height="100" style="object-fit:cover; border-radius:50%"> | **Kchibal <br> Ismail** <br> <img src="https://github.com/DApp-for-Real-Estate-Rental-on-Ethereum/.github/blob/main/profile/kchibal.jpeg" width="100" height="100" style="object-fit:cover; border-radius:50%"> | 
| **Role** | Backend Engineer | Frontend Engineer | Blockchain Engineer | DevOps Engineer / AI & Data Engineer | Cloud Engineer |
| **Description** | Spring Boot, REST APIs, DB Integration | Next.js Components, Web3 Integration, UX | Smart Contracts, Web3, Testnets | CI/CD Pipelines, Docker, orchestration, AI Pricing Models, Data Trends | AWS Infrastructure, Security, Storage |

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
