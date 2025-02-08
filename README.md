# Static Website Deployment on AWS 

## Problem Statement  

This project involves deploying a **static website** on **AWS infrastructure** for a client.  
The website content is stored in a **Git repository** and needs to be synchronized with an **Amazon S3 bucket** for scalability and reliability.  
The deployment utilizes an **AWS EC2 instance running Linux** as the web server.  

---

## Project Overview  

The goal of this project is to:  
✅ Set up an **EC2 instance** to host the website  
✅ Install and configure a **web server** (Apache)  
✅ Clone the **Git repository** containing the website files  
✅ Deploy the website on the **EC2 instance**  
✅ Sync the content with an **Amazon S3 bucket**  
✅ Ensure website availability via the **EC2 public IP or domain name**  

---

## Requirements  

### 1️⃣ Setup EC2 Instance  
- Launch an **AWS EC2 instance** with **Linux** as the OS  
- Configure **security groups** to allow inbound traffic:  
  - **HTTP (port 80)** for web access  
  - **SSH (port 22)** for remote access  

### 2️⃣ Install Web Server  
- Install and configure **Apache** to serve static files  
- Ensure **Apache** starts automatically on system boot  

### 3️⃣ Clone Git Repository  
- Install **Git** on the EC2 instance  
- Clone the repository containing the static website files  

### 4️⃣ Deploy Static Website  
- Move the cloned website files to the **web server's root directory**  
- Restart the web server to apply changes  

### 5️⃣ Setup Amazon S3 Bucket  
- Create an **S3 bucket** to host the static website  
- Configure **public read access** for the bucket  

### 6️⃣ Sync Content with S3  
- Use the **AWS CLI** to sync the EC2 web server files with the **S3 bucket**  
- Ensure that any updates in the Git repository are reflected in **S3**  

### 7️⃣ Testing and Validation  
- Verify website accessibility via **EC2 public IP** or **domain name**  
- Ensure changes pushed to the **Git repository** are updated in both the **EC2 instance** and **S3 bucket**  

---

🎯 **Project By:** [Sadika]   
