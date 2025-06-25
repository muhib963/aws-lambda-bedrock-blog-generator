# aws-lambda-bedrock-blog-generator
aws-lambda-bedrock-blog

# 📝 Blog Generator with AWS Lambda & Amazon Bedrock

This project is a **serverless blog generator** that uses **Amazon Bedrock** to generate a 200-word blog based on a given topic using **Meta Llama 3**, and saves the output to an **S3 bucket**. The logic is implemented in **Python** and deployed using **AWS Lambda**.

---

## Features

- Generates blog content using `meta.llama3-70b-instruct-v1:0` via Amazon Bedrock.
- Uses AWS Lambda for serverless execution.
- Saves generated content to Amazon S3 for persistence.
- Easily testable via API Gateway or Lambda Console.
- Lightweight and minimal dependencies.

---

## Architecture

```text
[Client or API Gateway]
          ↓
     [AWS Lambda]
          ↓
  [Amazon Bedrock (Llama3)]
          ↓
     [Amazon S3 Storage]
