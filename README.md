﻿# 📝 AWS Lambda Blog Generator using Amazon Bedrock

This project is a **serverless AWS Lambda function** that generates a 200-word blog using **Amazon Bedrock** with the `meta.llama2-13b-chat-v1` model and saves the output to an **S3 bucket**.

## 🚀 Features

- Accepts a blog topic via API Gateway.
- Uses Amazon Bedrock Model to generate the blog.
- Saves the generated content to a specified S3 bucket.
- Logs and handles errors gracefully.

---
## 🧪 How It Works

1. Triggered via HTTP request (API Gateway).
2. Sends a prompt to the Bedrock model 
3. Stores the generated blog in S3 bucket.

---

## 🔧 Prerequisites

- AWS account with:
  - Access to Amazon Bedrock.
  - Access to `meta.llama2-13b-chat-v1` model.
  - S3 bucket created (e.g., `aws_bedrock_course1`).
- Lambda execution role with:
  - `bedrock:InvokeModel`
  - `s3:PutObject`

---

## 🖼️ Setup Screenshots

- Lambda function setup
  ![image](https://github.com/user-attachments/assets/d31f8b53-79e3-45ee-9a1c-4cd3634a1910)
  
- API Gateway trigger
  ![Screenshot 2025-05-14 132223](https://github.com/user-attachments/assets/4f2f2a6a-b567-4c86-bfab-a6b6e3c09cd3)

- S3 upload confirmation
  ![image](https://github.com/user-attachments/assets/7da4567e-091d-4aec-8ad7-bf19fd8d4be0)




