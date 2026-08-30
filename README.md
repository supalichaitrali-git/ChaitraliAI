# ChaitraliAI 🤖

AI Voice Interview Agent representing **Chaitrali Supali**.

ChaitraliAI is a web-based AI interview agent designed to simulate a natural interview conversation and answer questions about Chaitrali's education, technical skills, projects, and experience.

The application uses a **FastAPI backend**, **Google Gemini API** for AI-generated responses, and a web-based frontend that communicates with the backend through HTTPS.

---

## 🚀 Live Application

**Backend API:**

https://chaitraliai.onrender.com

**API Documentation:**

https://chaitraliai.onrender.com/docs

**OpenAPI Specification:**

https://chaitraliai.onrender.com/openapi.json

---

## ✨ Features

- 🤖 AI-powered interview conversation
- 🎤 Voice-interview oriented frontend
- 💬 Natural conversational responses
- 👩‍💻 Answers questions about Chaitrali's:
  - Education
  - Technical skills
  - Projects
  - Experience
  - Career interests
- 🧠 Conversation history during an interview session
- 🔄 Interview reset functionality
- 📝 Interview session logging
- ❤️ Backend health-check endpoint
- 🌐 HTTPS deployment using Render
- 🔐 API key stored using environment variables
- 📡 REST API built with FastAPI
- ⚡ Gemini-powered dynamic responses
- 🛡️ Local fallback responses for selected basic questions

---

## 🏗️ Architecture

```text
                    ┌─────────────────────┐
                    │      User           │
                    │  Laptop / Phone     │
                    └──────────┬──────────┘
                               │
                               │ HTTPS
                               ▼
                    ┌─────────────────────┐
                    │      Frontend       │
                    │   Web Interface     │
                    └──────────┬──────────┘
                               │
                               │ REST API
                               ▼
                    ┌─────────────────────┐
                    │   FastAPI Backend   │
                    │     main.py         │
                    └──────────┬──────────┘
                               │
                 ┌─────────────┴─────────────┐
                 │                           │
                 ▼                           ▼
        ┌─────────────────┐         ┌─────────────────┐
        │ Local Responses │         │  Google Gemini  │
        │ Basic Questions │         │   AI Responses  │
        └─────────────────┘         └─────────────────┘
