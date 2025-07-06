# 🚀 AI Research Assistant

![MIT License](https://img.shields.io/badge/License-MIT-green.svg) ![Python 3.12+](https://img.shields.io/badge/Python-3.12%2B-blue.svg) ![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-orange.svg) ![FastAPI](https://img.shields.io/badge/Backend-FastAPI-lightgrey.svg)

> **AI Research Assistant** is a next-gen platform for immersive, AI-driven document analysis. Upload PDFs of research papers or reports, ask complex questions, and get precise, source-backed answers—all within a sleek, 3D glassmorphic UI.


## 🌟 Key Features

| Feature                | Description                                                                    |
| ---------------------- | ------------------------------------------------------------------------------ |
| 🖼️ 3D Immersive UI    | Glassmorphism cards, floating panels, and parallax effects for a modern UX     |
| 📄 PDF Intelligence    | Chunk, embed, and index PDFs for lightning-fast retrieval                      |
| 🤖 Gemini AI Powered   | Google Gemini via `google-generativeai` for top-tier RAG responses             |
| ❓ Smart Q\&A           | Multi-turn conversation, source citations, and context retention               |
| 📊 Performance Metrics | Live dashboard for ingestion time, latency, token usage, and confidence scores |
| 🔄 Session History     | Persistent chat logs and easy session resets                                   |
| 📱 Responsive Design   | Fully functional on desktop and mobile                                         |

---

## 🛠️ Tech Stack

```yaml
backend:
  framework: FastAPI + Uvicorn
  language: Python 3.12+
  vector_db: ChromaDB
  embeddings: HuggingFace
  ai_sdk: google-generativeai (Gemini)
  orchestration: LangChain
frontend:
  framework: Streamlit
  styling: CSS (Glassmorphism, 3D transforms)
infrastructure:
  container: Docker-ready
  deployment: Vercel (frontend) + any cloud VM (backend)
```

---

## 🚀 Quick Start

### 1. Clone & Setup

```bash
git clone https://github.com/your-username/AI-Research-Assistant.git
cd AI-Research-Assistant
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\\Scripts\\activate       # Windows
pip install --upgrade pip
pip install -r requirements.txt
```

### 2. Configure API Key

1. Copy `.env.example` to `.env`:

   ```bash
   cp .env.example .env
   ```
2. Add your Google Gemini API key:

   ```dotenv
   GEMINI_API_KEY=your_api_key_here
   ```

### 3. Run Locally

* **Backend**: `uvicorn app:app --reload --port 8000`
* **Frontend**: `streamlit run streamlit_app.py --server.port 8501`

> Now browse [http://localhost:8501](http://localhost:8501) and start analyzing documents!

---

## 🖥️ Usage Overview

1. **Upload PDF**: Click "Choose a PDF" and select your file.
2. **Process**: Hit "Process Document" to chunk and embed.
3. **Ask Gemini**: Type your question and click "Ask Gemini".
4. **Review**: View answers with inline citations, confidence, and performance stats.
5. **History & Reset**: Browse past Q\&A or click "Clear Document" to start anew.

---

## 📈 Metrics Dashboard

* **Ingest Time**: \~5s for 20-page PDF
* **Query Latency**: <2s per request on free-tier
* **Token Efficiency**: Optimized chunking to reduce cost

---

## 🤝 Contributing

1. 🌱 Fork the repository
2. 🛠️ Create a branch: `git checkout -b feature/my-new-feature`
3. 📝 Commit: `git commit -m "Add awesome feature"`
4. 📤 Push: `git push origin feature/my-new-feature`
5. 🔀 Open PR and describe your changes

Contributions should include tests and adhere to PEP8.

---

## 📜 License

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.

---

<p align="center">Built with ❤️ by the AI Research Community</p>
