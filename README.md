# 🚀 Serverless AI Chatbot on AWS

![AWS](https://img.shields.io/badge/AWS-Serverless-orange?style=for-the-badge&logo=amazonaws)
![Lambda](https://img.shields.io/badge/AWS-Lambda-FF9900?style=for-the-badge&logo=awslambda)
![API Gateway](https://img.shields.io/badge/API-Gateway-FF4F8B?style=for-the-badge)
![DynamoDB](https://img.shields.io/badge/Database-DynamoDB-blue?style=for-the-badge&logo=amazondynamodb)
![Bedrock](https://img.shields.io/badge/AI-Amazon%20Bedrock-purple?style=for-the-badge)
![Architecture](https://img.shields.io/badge/Architecture-Serverless-success?style=for-the-badge)

> A fully serverless, scalable AI-powered chatbot built using modern cloud-native architecture on AWS.

---

## 📌 Overview

This project is a production-style **AI Chatbot application** built using a fully serverless architecture.  
It integrates authentication, conversation session management, persistent chat history, and AI model invocation using managed AWS services.

The system is designed to be:

- ⚡ Scalable
- 💰 Cost-efficient (Pay-per-use)
- 🧩 Modular
- 🔄 Event-driven
- ☁️ Cloud-native

---

## 🧠 Tech Stack

**Cloud Platform**
- Amazon Web Services (AWS)

**Backend**
- AWS Lambda
- API Gateway
- DynamoDB
- Amazon Bedrock

**Frontend**
- HTML
- CSS
- JavaScript

**Hosting**
- Amazon S3 (Static Website Hosting)

---

# 🎥 Demo Video

🎬 Watch the complete working demo here:

👉 **[Watch Demo Video](https://drive.google.com/file/d/1753eX1adItd0djok-4-VdYvEdi9Ur0V2/view?usp=share_link)**

---

# 🌐 Live Application

🔗 Live Chatbot URL: http://chatbot-bucket-shivani.s3-website-us-east-1.amazonaws.com


---

# 🏗️ Architecture Overview

This application follows a **microservices-inspired serverless architecture**.

## 🔹 Lambda Functions (5)

| Function Name | Responsibility |
|--------------|---------------|
| Register | Stores new user in database |
| Login | Validates user credentials |
| Generate Conversation ID | Creates unique chat session |
| Model Invocation | Invokes AI model via Bedrock |
| History Fetch | Retrieves past conversations |

---

## 🔹 API Gateways (2)

### 1️⃣ Authentication Gateway
- Register API
- Login API
- Generate Conversation ID API

### 2️⃣ Chatbot Gateway
- Bedrock Invoke API
- History API

This separation ensures:
- Clear responsibility boundaries
- Modular backend
- Better scalability
- Clean architecture design

---

## 🔹 Database Layer

### 1️⃣ User Data Table (DynamoDB)

Stores:
- user_id (Primary Key)
- name
- email
- password

### 2️⃣ Conversation Data Table (DynamoDB)

Stores:
- conversation_id
- user_id
- user_message
- bot_response
- timestamp

---

# 🖼️ Architecture Diagram

![Architecture Diagram](<img width="689" height="349" alt="architecture-chatbot -shivani" src="https://github.com/user-attachments/assets/195f7c90-8aba-4f3d-ac63-245af780d249" />
)

🛠 **Future Improvements:**

- JWT-based authentication
- Password hashing & encryption
- Rate limiting
- Multi-model selection
- CI/CD pipeline
- CloudFormation / Terraform Infrastructure as Code
  
👩‍💻 **Author:**

Shivani Pandey
Cloud & Full Stack Developer

**⭐ If You Like This Project
Give it a ⭐ on GitHub and feel free to fork it!**



