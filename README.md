👨‍💻 Author

HarmeetKaur31

# AWS Three Tier Web Architecture

This project demonstrates a **3-tier AWS architecture** with secure networking and separation of concerns.

---

## 🏗️ Architecture Components

### 1. Web Tier (Frontend)
- React.js application
- Runs in public subnet (via Nginx in production)
- Accessible through Load Balancer

---

### 2. Application Tier (Backend)
- Node.js REST API
- Runs in private subnet (no public access)
- Handles business logic

---

### 3. Database Tier
- Amazon RDS (MySQL)
- Fully private subnet
- Only App Tier can access it

---

### 4. Bastion Host (Jump Server)
- EC2 instance in public subnet
- Used to SSH into private App Tier
- Secure access gateway (no direct internet access to App Tier)

---

## 🔐 Security Flow

- Users → Load Balancer → Web Tier → App Tier → Database
- Admin access: Laptop → Bastion Host → App Tier

---

## ⚙️ Tech Stack

- React.js
- Node.js
- MySQL (RDS)
- AWS EC2
- AWS VPC (Subnets, Security Groups)
- Nginx (Web serving)
- Bastion Host (SSH access control)

---

## 🔑 Bastion Host Access

```bash
ssh -i key.pem ec2-user@<bastion-public-ip>
ssh ec2-user@<app-private-ip>





