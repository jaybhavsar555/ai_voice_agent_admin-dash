# 🎙️ VoiceAgent AI - Admin Dashboard

A premium, high-performance administrative platform for managing and monitoring the **Sarah AI Voice Agent**. This dashboard provides real-time control over personas, knowledge bases, and automated calling campaigns.

---

## ✨ Core Features

### 📊 Call Log Viewer
- **Real-time Monitoring**: Track every call as it happens.
- **Detailed Transcripts**: Full conversational breakdown between the AI (Sarah) and customers.
- **Metrics**: Automated tracking of call duration, intent, and outcome.

### 🎭 Domain Configuration
- **Persona Management**: Edit Sarah's script and tone for different industries (Loans, Insurance, etc.).
- **Hot-Swapping**: Update the AI's behavior instantly from the browser without restarting the backend.

### 🧠 Knowledge Base (RAG)
- **Instant Training**: Add new facts and Q&A pairs directly to the Faiss vector database.
- **Enhanced Accuracy**: Improve Sarah's responses by providing specific business details.

### 🚀 Campaign Manager
- **Automated Dialing**: Upload contact lists via CSV and trigger massive outbound call runs.
- **Status Tracking**: Monitor campaign progress and success rates in real-time.

### 🔐 Secure Authentication
- **JWT Protection**: Secure, token-based login for internal team members.
- **Admin Access Control**: Role-based access to sensitive administrative data.

---

## 🛠️ Technology Stack

### Frontend
- **Framework**: [React](https://reactjs.org/) + [Vite](https://vitejs.dev/)
- **Styling**: Modern CSS with **Glassmorphism** & **Dark Mode**.
- **Icons**: [Lucide React](https://lucide.dev/)
- **State Management**: React Hooks & LocalStorage Persistence.

### Backend
- **API Framework**: [FastAPI](https://fastapi.tiangolo.com/) (Python)
- **Voice Pipeline**: [Pipecat](https://pipecat.ai/)
- **Database**: [MongoDB](https://www.mongodb.com/) (Motor Async)
- **Vector Search**: [Faiss](https://github.com/facebookresearch/faiss)
- **Telephony**: Twilio Integration.

---

## 🚀 Getting Started

### 1. Backend Setup
1. Navigate to the backend directory: `C:\ai_voice_agent\ai_voice_agent_app`
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Start the server:
   ```bash
   uvicorn app.server.main:app --host 0.0.0.0 --port 8000
   ```

### 2. Frontend Setup
1. Navigate to the dashboard directory: `c:\ai_voice-agent_admin_dash`
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file:
   ```env
   VITE_API_BASE_URL=http://localhost:8000
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```

---

## 🔑 Default Credentials
For the internal team:
- **Username**: `admin`
- **Password**: `voice123`

---

## 📁 Project Structure

```
ai_voice-agent_admin_dash/
├── src/
│   ├── components/       # Reusable UI components (Sidebar, Modals)
│   ├── pages/            # Page modules (CallLogs, Campaigns, etc.)
│   ├── App.jsx           # Main routing and Auth logic
│   └── index.css         # Global Premium Design System
├── .env                  # Backend configuration
└── package.json          # Dependency management
```
