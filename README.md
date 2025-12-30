# 🌐 Static Portfolio Website on AWS S3 (Terraform)

This repository contains the source code and infrastructure configuration for **Kshitija Randive’s personal portfolio website**, hosted as a **static website on AWS S3** and provisioned using **Terraform**.

The project demonstrates **real-world DevOps practices** such as Infrastructure as Code (IaC), clean Git workflows, and modern AWS S3 configuration without legacy ACLs.

---

## 🧠 Project Overview

- **Type**: Static portfolio website
- **Purpose**: Personal branding & recruiter showcase
- **Hosting**: AWS S3 Static Website
- **Provisioning**: Terraform
- **Security Model**: Bucket Policy (ACL-free, modern AWS best practice)

---

## 🛠️ Tech Stack

- **AWS S3** – Static website hosting  
- **Terraform** – Infrastructure as Code  
- **HTML & CSS** – Frontend  
- **Git & GitHub** – Version control  

---

## 📂 Repository Structure

.
├── index.html          # Main portfolio webpage
├── error.html          # Custom error page (404)
├── profile.png         # Profile image
├── main.tf             # Terraform resources
├── provider.tf         # AWS provider configuration
├── variables.tf        # Terraform variables
├── .gitignore          # Git ignore rules
└── README.md           # Project documentation

---

## ✨ Website Features

- Modern, responsive UI
- Clean CSS animations
- Project showcase section
- Reviews/testimonials section
- Custom error page
- Profile image integration
- Lightweight & fast loading

---

## 🧱 Infrastructure Details

Terraform provisions the following AWS resources:

- S3 bucket
- Bucket ownership controls (ACLs disabled)
- Public access configuration
- Bucket policy for public read access
- Static website configuration
- Object uploads (index.html, error.html, assets)

### 🔐 Why No ACLs?
ACLs are deprecated for most use cases.  
This project uses **bucket policies** instead, which is the **AWS-recommended and production-safe approach**.

---

## 🚀 Deployment Steps

### 1️⃣ Prerequisites
- AWS Account
- AWS CLI configured
- Terraform installed

### 2️⃣ Initialize Terraform
terraform init

### 3️⃣ Validate Configuration
terraform validate

### 4️⃣ Deploy Infrastructure
terraform apply -auto-approve

Once applied, the website will be accessible using the S3 website endpoint.

---

## 🔒 Security & Best Practices

- No hardcoded credentials
- .terraform directory excluded from Git
- Terraform state files ignored
- Fully reproducible infrastructure
- Clean Git history

---

## 👩‍💻 About Me

**Kshitija Randive**  
DevOps Engineer with hands-on experience in AWS, GCP, CI/CD pipelines, Terraform, Docker, Kubernetes, and cloud automation.

---

## 📄 License

This project is intended for personal and educational use.
