# 🧠 LLaMA Text Summarizer

An AI-powered text summarization app that uses **LLaMA 2** (via Ollama) for generating concise summaries. Built with a **FastAPI backend** and a **Streamlit frontend**.

---

## 🚀 Features

- Summarizes long texts using the LLaMA 2 model
- Simple and user-friendly Streamlit interface
- FastAPI backend to handle summarization requests
- Runs fully locally using [Ollama](https://ollama.com/) – no need for external APIs

---

## 📦 Tech Stack

- **Frontend:** Streamlit
- **Backend:** FastAPI
- **LLM Runtime:** Ollama
- **Language Model:** LLaMA 2
- **HTTP Requests:** Python `requests` library

---

## ⚙️ Setup Instructions

1. Clone the repo
2. Install dependencies: `pip install -r requirements.txt`
3. Run backend: `uvicorn backend.main:app --reload`
4. Run frontend: `streamlit run frontend/app.py`
