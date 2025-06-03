🧠 LLaMA Text Summarizer
An AI-powered text summarization app that uses LLaMA 2 (via Ollama) for generating concise summaries. Built with a FastAPI backend and a Streamlit frontend.

🚀 Features
Summarizes long texts using the LLaMA 2 model

Simple and user-friendly Streamlit interface

FastAPI backend to handle summarization requests

Runs fully locally using Ollama – no need for external APIs

📦 Tech Stack
Frontend: Streamlit | Backend: FastAPI | LLM Runtime: Ollama | Language Model: LLaMA 2 | HTTP Requests: Python requests library

⚙️ Setup Instructions
Clone the repository:

git clone https://github.com/your-username/llama-text-summarizer.git
cd llama-text-summarizer

Create and activate a Python virtual environment:

python -m venv venv
# On macOS/Linux:
source venv/bin/activate
# On Windows (PowerShell):
.\venv\Scripts\Activate.ps1
# Or Windows (CMD):
.\venv\Scripts/activate.bat

Install required Python packages:

pip install -r requirements.txt

If you don't have a requirements.txt file, install dependencies manually:

pip install fastapi uvicorn streamlit requests python-multipart

Install Ollama and download LLaMA 2 model:
Download and install Ollama from https://ollama.com
Then, pull the LLaMA 2 model locally:

ollama pull llama2

▶️ Running the Application
Start the FastAPI backend server:

uvicorn backend.main:app --reload

In a new terminal, start the Streamlit frontend:

streamlit run frontend/app.py

Open your browser to http://localhost:8501.

📝 Usage
Simply enter or paste any long text into the input box on the Streamlit page and click "Summarize". The backend will send your text to LLaMA 2 running in Ollama and display the generated summary below the input box.

📁 Project Structure
llama-text-summarizer/
├── backend/
│   ├── __init__.py
│   └── main.py          # FastAPI application
├── frontend/
│   └── app.py           # Streamlit application
├── venv/                # Virtual environment
├── requirements.txt     # Python dependencies
└── README.md            # This file

🛠️ API Endpoints
POST /summarize
Summarizes the provided text using LLaMA 2.

Request Body Example:

{
  "text": "Your long text to summarize..."
}

Response Example:

{
  "summary": "Generated summary of the text"
}

🐛 Troubleshooting
uvicorn or streamlit command not found: Ensure your virtual environment is activated and dependencies (uvicorn, fastapi, streamlit) are installed.

Ollama connection error: Verify that Ollama is running (ollama serve) and the LLaMA 2 model is downloaded (ollama pull llama2).

Port already in use: If a port is already in use, kill existing processes or specify a different port (e.g., uvicorn backend.main:app --reload --port 8001 or streamlit run frontend/app.py --server.port 8502).

📋 Requirements
Python 3.8+

Ollama installed and running

LLaMA 2 model downloaded via Ollama
