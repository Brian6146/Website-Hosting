# 🌐 AWS EC2 Website Hosting Project

This project demonstrates how I deployed a simple website using **Amazon EC2**. I manually launched and configured an Ubuntu-based EC2 instance, installed the Apache web server, adjusted security settings, assigned an Elastic IP, and deployed a custom HTML file using the terminal.

---

## 📁 Project Overview

The goal of this project was to gain hands-on experience in:
- Launching and configuring an AWS EC2 instance
- Assigning an Elastic IP to maintain a static address
- Installing and running a web server (Apache2)
- Managing security groups for HTTP access
- Hosting a custom HTML page using Apache

---

## 🚀 Technologies Used

- **Amazon Web Services (AWS)**
- **EC2 (Elastic Compute Cloud)**
- **Elastic IP**
- **Ubuntu Server (20.04)**
- **Apache2 Web Server**
- **nano (CLI text editor)**

---

## 🔧 Steps I Followed

### 1. **Launched EC2 Instance**
- Selected **Ubuntu Server 20.04 LTS** as the OS.
- Chose a **t2.micro** instance (eligible for free tier).
- Created a new key pair for SSH access.

### 2. **Configured Security Groups**
- Allowed inbound traffic for:
  - **SSH (port 22)** – to connect to the instance
  - **HTTP (port 80)** – to serve web pages

### 3. **Set Up an Elastic IP**
- Allocated a new **Elastic IP** from the AWS EC2 dashboard.
- Associated the Elastic IP with my running instance.
- This ensures the public IP remains **static** across restarts.

### 4. **Connected to the Instance**
- Used SSH to connect:

  ```bash
  ssh -i your-key.pem ubuntu@<your-elastic-ip>


