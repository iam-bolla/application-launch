# 🌐 Java Hello World Web Server on AWS EC2

This is a lightweight Java HTTP server that returns "Hello, World!" on browser access. This guide walks you through running it on your local machine and deploying it to an AWS EC2 instance.

---

## ✅ 1. Tools & Requirements

- **Java Development Kit (JDK)**: Install Java 17 or later
- **AWS Account**
- **EC2 Instance**: Amazon Linux or Ubuntu
- **Security Group Rule**: Allow inbound traffic on port **8080** (or use port **80**)

---

## ✅ 2. Steps to Run on AWS EC2

### 🔹 Local Machine Setup

1. **Save the Code**

Save the Java server code as `HelloWorldServer.java`.

2. **Compile**

```bash
javac HelloWorldServer.java
Run Locally for Testing

java HelloWorldServer
Check Output in Browser
```
Visit:
http://localhost:8080
---
🔹 AWS EC2 Deployment
Launch an EC2 Instance

Use Amazon Linux or Ubuntu

Allow port 8080 in the Security Group settings

SSH into the Instance

```bash
ssh -i your-key.pem ec2-user@<your-ec2-ip>
```
Install Java on EC2

For Ubuntu:

```bash
sudo apt update
sudo apt install default-jdk -y
```

clone the repo into instance
```bash
git clone repo-link
```
Compile and Run on EC2

```bash
javac HelloWorldServer.java
java HelloWorldServer
```
Access the App

Visit in browser:
```bash
http://<EC2-Public-IP>:8080
```
You should see:
```bash
Hello, World from SRAVYA!
```
Optional: Auto-start with Systemd or Run in Background
To run in the background:
```bash
nohup java HelloWorldServer &
```
