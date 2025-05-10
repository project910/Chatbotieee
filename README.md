# 💼 AI-Powered Financial Assistant with RAG and Flutter Chatbot

This project is a smart system that combines **AI**, **data retrieval**, and **task automation** to help users manage and query their financial data (invoices, transactions, etc.). It features a **Retrieval-Augmented Generation (RAG)** model, a backend **API**, and a user-facing **Flutter chatbot**.

---

## 🚀 Features

- Natural language understanding for financial queries.
- Real-time answers using a RAG system.
- User-specific knowledge base.
- Secure API with endpoints for data input, reporting, and notifications.
- Mobile chatbot interface using Flutter.
- Hosted API on Render.
- Multi-user architecture with isolated data per user.

---

## 🛠️ Project Components

### 1. Requirements Analysis
- Identified the types of financial data to be handled (e.g., invoices, transactions).
- Defined common user queries (e.g., "What did I spend in April?").
- Determined key automated features: notifications, expense categorization, downloadable reports.

---

### 2. Data Preparation
- Collected and cleaned structured financial data (CSV, Excel).
- Vectorized the cleaned data using:
  - `OpenAI Embeddings`.

---

### 3. Knowledge Base Construction
- Built a vector database using `FAISS` or `Chroma`.
- Created a multi-tenant setup: each user's data is stored and accessed independently.
- Implemented a retrieval system that brings back relevant context for user queries.

---

### 4. RAG Model Integration
- Connected a language model to the vector database.
- Implemented a system for Retrieval-Augmented Generation to answer user questions.
- Evaluated the model's response quality and improved retrieval accuracy.

---

### 5. Backend API Development
- Developed the backend using **FastAPI**.
- Created endpoints for:
  - Uploading and managing financial data.
  - Querying the RAG model.
  - Downloading reports.
  - Managing notifications and user settings.
- Hosted the API on **Render**.
- Pushed source code to **GitHub** for version control and collaboration.

---

### 6. Flutter Chatbot UI
- Built a mobile app using **Flutter**.
- Integrated it with the backend API to support user queries via chat.
- Provided features like:
  - User login & authentication.
  - Real-time notifications.
  - Report downloading.
  - Simple and intuitive financial insights via chat.

---

## 📦 Deliverables

- Full-stack AI-powered assistant for financial data management.
- Hosted API ready for production use.
- Mobile-friendly chatbot interface.
- Easily extendable for more financial operations or enterprise-level features.

---

## 🧠 Tech Stack

- **Python** (FastAPI, OpenAI API)
- **Flutter** (for the frontend chatbot)
- **Render** (API hosting)
- **FAISS / Chroma** (vector database)
- **OpenAI Embeddings** (vectorization)
- **GitHub** (code management)

---

## 📁 Repository Structure

```bash
.
├── api/                # FastAPI backend code
├── flutter_app/        # Flutter mobile app
├── data/               # Sample financial datasets
├── embeddings/         # Vectorization logic
├── models/             # RAG and related logic
├── utils/              # Helper functions and scripts
└── README.md           # Project documentation

