# 🧠 LLaMA Text Summarizer

An AI-powered text summarization app that uses LLaMA 2 (via Ollama) for generating concise summaries. Built with a FastAPI backend and a Streamlit frontend.

---

## 🚀 Features

* Summarizes long texts using the **LLaMA 2 model**
* Simple and user-friendly **Streamlit interface**
* **FastAPI backend** to handle summarization requests
* Runs **fully locally** using Ollama – no need for external APIs

---

## 📦 Tech Stack

**Frontend**: Streamlit | **Backend**: FastAPI | **LLM Runtime**: Ollama | **Language Model**: LLaMA 2 | **HTTP Requests**: Python `requests` library

---

## ⚙️ Setup Instructions

1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/your-username/llama-text-summarizer.git](https://github.com/your-username/llama-text-summarizer.git)
    cd llama-text-summarizer
    ```

2.  **Create and activate a Python virtual environment**:
    ```bash
    python -m venv venv
    # On macOS/Linux:
    source venv/bin/activate
    # On Windows (PowerShell):
    .\venv\Scripts\Activate.ps1
    # Or Windows (CMD):
    .\venv\Scripts/activate.bat
    ```

3.  **Install required Python packages**:
    ```bash
    pip install -r requirements.txt
    ```
    If you don't have a `requirements.txt` file, install dependencies manually:
    ```bash
    pip install fastapi uvicorn streamlit requests python-multipart
    ```

4.  **Install Ollama and download LLaMA 2 model**:
    Download and install Ollama from [https://ollama.com](https://ollama.com)
    Then, pull the LLaMA 2 model locally:
    ```bash
    ollama pull llama2
    ```

---

## ▶️ Running the Application

1.  **Start the FastAPI backend server**:
    ```bash
    uvicorn backend.main:app --reload
    ```

2.  **In a new terminal, start the Streamlit frontend**:
    ```bash
    streamlit run frontend/app.py
    ```
    Open your browser to `http://localhost:8501`.

---

## 📝 Usage

Simply enter or paste any long text into the input box on the Streamlit page and click "Summarize". The backend will send your text to LLaMA 2 running in Ollama and display the generated summary below the input box.

---

## 📁 Project Structure
Markdown

# 🧠 LLaMA Text Summarizer

An AI-powered text summarization app that uses LLaMA 2 (via Ollama) for generating concise summaries. Built with a FastAPI backend and a Streamlit frontend.

---

## 🚀 Features

* Summarizes long texts using the **LLaMA 2 model**
* Simple and user-friendly **Streamlit interface**
* **FastAPI backend** to handle summarization requests
* Runs **fully locally** using Ollama – no need for external APIs

---

## 📦 Tech Stack

**Frontend**: Streamlit | **Backend**: FastAPI | **LLM Runtime**: Ollama | **Language Model**: LLaMA 2 | **HTTP Requests**: Python `requests` library

---

## ⚙️ Setup Instructions

1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/your-username/llama-text-summarizer.git](https://github.com/your-username/llama-text-summarizer.git)
    cd llama-text-summarizer
    ```

2.  **Create and activate a Python virtual environment**:
    ```bash
    python -m venv venv
    # On macOS/Linux:
    source venv/bin/activate
    # On Windows (PowerShell):
    .\venv\Scripts\Activate.ps1
    # Or Windows (CMD):
    .\venv\Scripts/activate.bat
    ```

3.  **Install required Python packages**:
    ```bash
    pip install -r requirements.txt
    ```
    If you don't have a `requirements.txt` file, install dependencies manually:
    ```bash
    pip install fastapi uvicorn streamlit requests python-multipart
    ```

4.  **Install Ollama and download LLaMA 2 model**:
    Download and install Ollama from [https://ollama.com](https://ollama.com)
    Then, pull the LLaMA 2 model locally:
    ```bash
    ollama pull llama2
    ```

---

## ▶️ Running the Application

1.  **Start the FastAPI backend server**:
    ```bash
    uvicorn backend.main:app --reload
    ```

2.  **In a new terminal, start the Streamlit frontend**:
    ```bash
    streamlit run frontend/app.py
    ```
    Open your browser to `http://localhost:8501`.

---

## 📝 Usage

Simply enter or paste any long text into the input box on the Streamlit page and click "Summarize". The backend will send your text to LLaMA 2 running in Ollama and display the generated summary below the input box.

---

## 📁 Project Structure

llama-text-summarizer/
├── backend/
│   ├── init.py
│   └── main.py          # FastAPI application
├── frontend/
│   └── app.py           # Streamlit application
├── venv/                # Virtual environment
├── requirements.txt     # Python dependencies
└── README.md            # This file
