# 📄 RAG Based Intelligent Chatbot using Gemini & ChromaDB

A complete **Retrieval-Augmented Generation (RAG)** chatbot built from scratch using **Google Gemini**, **LangChain**, **ChromaDB**, and **PyPDF**.

This project allows users to ask questions about a PDF document. Instead of sending the entire PDF to the LLM, the system retrieves only the most relevant information and uses it to generate accurate answers.

---

# 🚀 Features

- 📄 Read PDF documents
- ✂️ Split documents into smaller chunks
- 🧠 Generate vector embeddings using Gemini Embedding Model
- 🗂 Store embeddings in ChromaDB
- 🔍 Retrieve the most relevant chunks using semantic search
- 🤖 Generate accurate answers using Gemini 2.5 Flash
- 📚 Beginner-friendly implementation with step-by-step explanation

---

# 🛠 Tech Stack

- Python
- Google Gemini API
- LangChain
- ChromaDB
- PyPDF
- Google Colab

---

# 📂 Project Workflow

```text
PDF
 │
 ▼
Read PDF
 │
 ▼
Extract Text
 │
 ▼
Chunking
 │
 ▼
Generate Embeddings
 │
 ▼
Store in ChromaDB
═══════════════════════════════

User Question
 │
 ▼
Question Embedding
 │
 ▼
Semantic Search
 │
 ▼
Top Relevant Chunks
 │
 ▼
Prompt Engineering
 │
 ▼
Gemini 2.5 Flash
 │
 ▼
Final Answer
```

---

# 📌 How RAG Works

Unlike a normal LLM, RAG does not answer directly from the model's knowledge.

Instead, it follows these steps:

1. Read the PDF.
2. Extract all text.
3. Split the text into smaller chunks.
4. Convert each chunk into vector embeddings.
5. Store embeddings inside ChromaDB.
6. Convert the user's question into an embedding.
7. Retrieve the most relevant chunks using cosine similarity.
8. Send the retrieved context and the question to Gemini.
9. Gemini generates the final answer.

---

# 📦 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/RAG-Based-Intelligent-Chatbot.git
```

Install dependencies

```bash
pip install pypdf
pip install langchain
pip install langchain-text-splitters
pip install langchain-google-genai
pip install langchain-chroma chromadb
```

---

# 🔑 API Key Setup

Create a Google Gemini API Key.

Store it inside Google Colab Secrets as:

```
GOOGLE_API_KEY
```

Then access it using:

```python
from google.colab import userdata

GOOGLE_API_KEY = userdata.get("GOOGLE_API_KEY")
```

---

# 📖 Project Steps

## Step 1

Read PDF using PyPDF.

## Step 2

Extract all text.

## Step 3

Split text into chunks.

## Step 4

Generate embeddings using:

```
models/gemini-embedding-2
```

## Step 5

Store embeddings in ChromaDB.

## Step 6

Convert the user's question into embeddings.

## Step 7

Retrieve the most relevant chunks.

## Step 8

Create the prompt.

## Step 9

Send the prompt to Gemini 2.5 Flash.

## Step 10

Generate the final answer.

---

# 💡 Example

### User Question

```
How many casual leaves are given?
```

### Retrieved Context

```
Employees are entitled to 18 casual leaves,
12 sick leaves,
and 15 earned leaves.
```

### Gemini Response

```
Employees are entitled to 18 casual leaves per year.
```

---

# 📁 Project Structure

```
RAG-Based-Intelligent-Chatbot
│
├── RAG_Based_Intelligent_Chatbot.ipynb
├── Employee_Handbook_Sample.pdf
├── README.md
└── requirements.txt
```

---

# 🎯 Future Improvements

- Upload multiple PDFs
- Chat history
- FastAPI Backend
- Streamlit / React Frontend
- Persistent Chroma Database
- Docker Support
- Cloud Deployment

---

# 📺 YouTube Tutorial

Complete step-by-step explanation available on YouTube.

**(Add your YouTube link here)**

---

# ⭐ If you found this project useful

Please consider giving this repository a ⭐ on GitHub.

It helps support future AI and Machine Learning projects.

---

## 👨‍💻 Author

**Ayush Agarwal**

AI / Machine Learning Engineer

GitHub: https://github.com/ayushagarwal13

LinkedIn: *(Add your LinkedIn Profile)*

YouTube: *(Add your YouTube Channel)*
