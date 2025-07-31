# 🌐 Java Hello World Web Server on AWS EC2

This is a lightweight Java HTTP server that returns "Hello, World!" on browser access. This guide walks you through running it on your local machine and deploying it to an AWS EC2 instance.

---

## ✅ 1. Tools & Requirements

- **Java Development Kit (JDK)**: Install Java 8 or later
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

Visit:
http://localhost:8080
