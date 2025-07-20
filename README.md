# 🧠 YouTube AI Chat Extension

Chat with any YouTube video using AI!  
This Chrome extension uses **Retrieval-Augmented Generation (RAG)** to let you ask questions based on the actual content being spoken in the video — powered by transcript extraction and generative AI.

---

## 🚀 Features

- 🔍 Ask questions about the content of any YouTube video
- 🤖 RAG-powered answers using real-time transcript retrieval
- 🎓 Great for tutorials, lectures, explainer videos, etc.
- 🌐 Works with most videos, including support for multilingual content (like Hindi-English mixes)
- 🔒 All communication is handled securely using your local backend and AI APIs

---

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS, JavaScript, Chrome Extension APIs
- **Backend:** FastAPI (Python)
- **AI Orchestration:** Langchain
- **LLM:** Google-gemini
- **Environment Handling:** `python-dotenv`

---


# 🔧 Setup Instructions: YouTube AI Chat Extension

This guide covers how to set up the **backend** (FastAPI) and the **Chrome Extension** for local use.

---

## 🛠️ Backend Setup (FastAPI)

1. **Navigate to the backend folder**:

```bash
cd backend
```

2. **Install dependencies**:

```bash
pip install -r requirements.txt
```

3. **Create a `.env` file** in the `backend/` folder and add your Google API key:

```
GOOGLE_API_KEY=your_google_genai_key_here
```

4. **Run the FastAPI server**:

```bash
uvicorn main:app --reload
```

> The server should run at `http://localhost:8000`

---

## 🧩 Chrome Extension Setup

1. Open Chrome and go to:

```
chrome://extensions/
```

2. **Enable Developer Mode** (toggle in the top right)

3. Click **"Load Unpacked"** and select the `extension/` folder

4. Open any YouTube video and click on the extension icon

5. Ask your question — the extension will communicate with the backend to get the answer

> Make sure the backend is running locally while using the extension.

---

## ✅ Done!

You’re all set to use the YouTube AI Chat Extension locally!
