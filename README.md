# 🎨 Deploy a Serverless Web Application to Edit Images Using Amazon Bedrock

**Amazon Bedrock Workshop 3 – Hands-on Implementation**

Generative AI has evolved beyond text-based applications. With Amazon Bedrock, it's now possible to build secure, scalable, and production-ready multi-modal applications that can generate and edit images using foundation models. In Workshop 3 of the Amazon Bedrock Workshop Series, I built and deployed a fully serverless web application that allows authenticated users to edit images using AI, powered by Titan Image Generator G1.

**Pavan Mali**  
*Published Dec 15, 2025*

---

## 🎨 Workshop Overview

Welcome to the Deploy a Serverless Web Application to Edit Images Using Amazon Bedrock workshop!

In this hands-on lab, I built a complete serverless image editing solution using AWS-managed services. The application includes:

- ✅ Secure user authentication
- ✅ AI-powered image generation and editing
- ✅ Persistent metadata storage
- ✅ RESTful APIs
- ✅ A modern web-based UI

All components are fully serverless, ensuring scalability, security, and minimal operational overhead.

---

## 🧱 Architecture Overview

The application follows a cloud-native serverless architecture with seamless integration between AWS services.
![Architecture Diagram](archi.png)

---

## 🧰 Technology Stack

| Component | Technology |
|-----------|-----------|
| **Authentication** | Amazon Cognito (User Pool & authentication) |
| **Database** | Amazon DynamoDB (image generation/edit metadata) |
| **Compute** | AWS Lambda (serverless business logic) |
| **API Layer** | Amazon API Gateway (REST endpoints) |
| **AI Services** | Amazon Bedrock with Titan Image Generator G1 |
| **Frontend** | AWS Amplify (web application hosting) |

---

## 🎯 Learning Objectives

By the end of this workshop, I was able to:

✅ Understand serverless architecture patterns  
✅ Implement secure authentication using Amazon Cognito  
✅ Design NoSQL data models using DynamoDB  
✅ Build REST APIs with API Gateway  
✅ Develop serverless logic using AWS Lambda  
✅ Integrate AI models using Amazon Bedrock  
✅ Deploy frontend applications using AWS Amplify  
✅ Generate and edit images using Titan Image Generator G1  

---

## 🧪 Hands-on Lab Implementation

### 1️⃣ User Authentication with Amazon Cognito

**Tasks Completed:**
- Created a Cognito User Pool
- Configured authentication flows
- Created test users
- Integrated Cognito with the frontend

🔐 This ensures only authenticated users can access image editing features.

---

### 2️⃣ Data Storage with Amazon DynamoDB

**Created a DynamoDB table to store:**
- User ID
- Image prompt
- Generated image reference
- Timestamp
- Used on-demand capacity for auto-scaling

📦 DynamoDB provides fast, scalable, serverless data storage.

---

### 3️⃣ Serverless Logic with AWS Lambda

**Lambda function handles:**
- Image edit requests
- Calls to Amazon Bedrock
- Response processing
- Writing metadata to DynamoDB

**IAM permissions configured for:**
- Bedrock access
- DynamoDB read/write

🧠 Lambda acts as the core AI execution layer.

---

### 4️⃣ API Layer with Amazon API Gateway

**Created REST APIs to:**
- Submit image edit requests
- Retrieve image history
- Secured APIs using Cognito Authorizer

🌐 API Gateway exposes Bedrock-powered functionality securely.

---

### 5️⃣ Frontend Deployment with AWS Amplify

**Built a simple web UI for:**
- User authentication
- Image upload
- Prompt-based editing

**Integrated Amplify with:**
- Cognito
- API Gateway
- Enabled CI/CD from GitHub

🎯 Amplify simplified frontend hosting and deployment.

---

### 6️⃣ Testing the End-to-End Application

**Workflow Validation:**
1. ✅ Logged in as a user
2. ✅ Uploaded an image
3. ✅ Entered an image editing prompt
4. ✅ Lambda invoked Titan Image Generator G1
5. ✅ Edited image returned successfully
6. ✅ Metadata stored in DynamoDB

✅ **End-to-end workflow validated successfully.**

---

## 🖼️ Final Output

The application successfully demonstrates image editing using Titan Image Generator G1 with capabilities including:

- **Inpainting** - Edit specific regions within images
- **Outpainting** - Extend images beyond original boundaries

---

## 🧠 Key Takeaways

- 🚀 Serverless + GenAI is a powerful combination
- 🤖 Amazon Bedrock simplifies AI integration
- 🔒 Cognito ensures secure access
- 📈 DynamoDB scales seamlessly
- ⚡ Amplify accelerates frontend deployment
- 🎨 Titan Image Generator G1 enables high-quality image editing

---

## 🚀 Conclusion

Workshop 3 demonstrated how to build a secure, scalable, and production-ready image editing application using Amazon Bedrock and AWS serverless services.

By combining:
- Amazon Bedrock
- AWS Lambda
- API Gateway
- Cognito
- DynamoDB
- Amplify

I successfully deployed a **real-world multi-modal GenAI application** without managing servers or infrastructure.

---

## 🙏 Acknowledgements

A big thank you to the **AWS Team** and **Hack2skill** for organizing and delivering such a well-structured and hands-on workshop.

Special thanks to:
- **Anannya Roy Chowdhury** for excellent guidance
- **Ashita Prasad** for clear explanations and continuous support

This session provided valuable real-world exposure to building serverless, AI-powered applications using Amazon Bedrock, and it was a truly enriching learning experience.

---

**Happy Learning! 🎉**
