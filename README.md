# 🤖 RAG Chatbot with Amazon Bedrock

A Retrieval-Augmented Generation (RAG) chatbot built using **Amazon Bedrock**, **Amazon OpenSearch Serverless**, and **Amazon S3**.  
This chatbot can answer questions from your own documents (e.g., HR policies, project knowledge base, or personal files) with accurate, context-aware responses.

---

## 🚀 Overview
AI chatbots like ChatGPT are powerful, but they can’t answer questions about your private data out of the box.  
This project uses **RAG (Retrieval-Augmented Generation)** to extend a Large Language Model (LLM) hosted on **Amazon Bedrock**, allowing it to retrieve relevant information from custom documents stored in **S3** and indexed in **OpenSearch**.

**Use case demo:**  
Here, the chatbot is specialized for **HR policies**, letting employees ask questions like:  
- “What are the vacation policies?”  
- “How does the performance review process work?”  
- “What healthcare benefits are available?”  
<img width="358.4" height="537.6" alt="112a0a36-b0a7-4ef0-b84f-38884b0312ba" src="https://github.com/user-attachments/assets/7c813169-aae3-487e-b52f-3e53b513556b" />

---

## 🛠️ Tech Stack
- **Amazon Bedrock** – Large Language Models (LLMs) for response generation  
- **Amazon S3** – Document storage for HR policies / custom knowledge base  
- **Amazon OpenSearch Serverless** – Vector search database for semantic retrieval  
- **Python (Boto3 SDK)** – Backend integration with AWS services  

---

## 🔄 Architecture

```text
User → Chatbot UI → Amazon Bedrock (LLM)
                     ↘ Retrieval (RAG)
                        → OpenSearch (Vector DB)
                            ↘ Amazon S3 (Document Store)

