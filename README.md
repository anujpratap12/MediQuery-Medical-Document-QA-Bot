# 🩺 MediQuery – Medical Document Q&A Bot

MediQuery is an AI-powered Medical Document Question Answering system built using Retrieval-Augmented Generation (RAG). The application allows users to upload medical PDF documents and ask context-aware questions using Large Language Models (LLMs).

The project follows a modern modular architecture using FastAPI for backend APIs and Streamlit for the frontend interface, making the system scalable, easy to maintain, and deployment-ready.

---

# 🚀 Features

* 📁 Upload and analyze multiple medical PDF documents
* 🧠 Context-aware question answering using RAG architecture
* 🔍 Semantic search with vector embeddings
* 💬 Interactive chatbot interface
* ⚡ FastAPI-powered backend APIs
* 🎨 Streamlit frontend with responsive UI
* 🔌 Support for Groq and Gemini LLM providers
* 🧪 Token-based document chunking for better retrieval
* 📦 Downloadable chat history
* 🔄 Reset and clear chat functionality
* 🔎 Query inspector for debugging and transparency
* 🌐 API-driven modular architecture

---

# 🏗️ System Architecture

The project is divided into two independent modules:

## 1. Frontend (Client)

Built using Streamlit.

Responsibilities:

* PDF upload interface
* Chat interface
* Chat history management
* Displaying responses
* Model selection
* User interaction handling

## 2. Backend (Server)

Built using FastAPI.

Responsibilities:

* Document processing
* Embedding generation
* Vector database operations
* Retrieval pipeline
* LLM response generation
* API endpoints

---

# 🧠 RAG Workflow

1. User uploads medical PDF documents
2. Backend extracts document text
3. Text is split into token-based chunks
4. Embeddings are generated
5. Chunks are stored inside vector database
6. User asks a question
7. Relevant chunks are retrieved
8. LLM generates context-aware answer
9. Response is displayed in chat interface

---

# 🛠️ Tech Stack

## Frontend

* Streamlit

## Backend

* FastAPI
* Uvicorn

## AI & RAG

* LangChain
* ChromaDB
* Google Gemini API
* Groq API

## Programming Language

* Python

---

# 📂 Project Structure

```bash
MediQuery-Medical-Document-QA-Bot/
│
├── client/
│   ├── components/
│   ├── state/
│   ├── utils/
│   ├── app.py
│   └── requirements.txt
│
├── server/
│   ├── api/
│   ├── config/
│   ├── core/
│   ├── utils/
│   ├── main.py
│   └── requirements.txt
│
├── assets/
├── README.md
├── LICENSE
└── .gitignore
```

---

# 📦 Installation Guide

## 1. Clone Repository

```bash
git clone https://github.com/anujpratap12/MediQuery-Medical-Document-QA-Bot.git
```

## 2. Open Project Folder

```bash
cd MediQuery-Medical-Document-QA-Bot
```

## 3. Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux / Mac

```bash
python3 -m venv venv
source venv/bin/activate
```

---

# 📥 Install Dependencies

## Install Frontend Dependencies

```bash
cd client
pip install -r requirements.txt
```

## Install Backend Dependencies

```bash
cd ../server
pip install -r requirements.txt
```

---

# 🔐 Environment Variables

Create a `.env` file inside the server directory.

Example:

```env
GROQ_API_KEY=your_groq_api_key
GOOGLE_API_KEY=your_google_api_key
```

---

# ▶️ Running the Application

## Start Backend Server

Open Terminal 1:

```bash
cd server
uvicorn main:app --reload
```

Backend runs on:

```bash
http://127.0.0.1:8000
```

---

## Start Frontend Application

Open Terminal 2:

```bash
cd client
streamlit run app.py
```

Frontend runs on:

```bash
http://localhost:8501
```

---

# 💡 Example Use Cases

* Medical report analysis
* Clinical document Q&A
* Healthcare document retrieval
* AI-powered medical assistant
* Patient report understanding
* Research paper querying

---

# 🔍 Core Functionalities

## 📁 Multi-PDF Upload

Users can upload multiple PDF files simultaneously for retrieval-based querying.

## 🧠 Intelligent Retrieval

Relevant chunks are retrieved using semantic similarity search.

## 💬 Conversational Chat

Users can interact with uploaded medical documents naturally.

## 🔎 Query Inspector

Displays retrieved chunks and metadata for transparency.

## 📦 Download Chat History

Users can export conversation history.

---

# ⚙️ API Endpoints

## Upload Documents

```bash
POST /upload
```

## Chat Query

```bash
POST /chat
```

## Reset Session

```bash
POST /reset
```

---

# 📈 Future Improvements

* 🔐 User authentication system
* ☁️ Cloud deployment
* 🗂️ Database integration
* 📱 Mobile-friendly UI
* 🧬 Medical terminology optimization
* 🎙️ Voice-based interaction
* 📊 Advanced analytics dashboard

---

# 👨‍💻 Developer

Anuj Pratap Singh

* AI/ML Enthusiast
* AI/ML Intern
* Final Year Engineering Student

---

# 🙌 Acknowledgements

This project was developed as part of learning and implementing modern Retrieval-Augmented Generation (RAG) systems using FastAPI, Streamlit, LangChain, and Vector Databases.


---

# ⭐ Support

If you found this project useful, consider giving it a star on GitHub.
