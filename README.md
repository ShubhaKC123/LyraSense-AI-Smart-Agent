# 🌟 LyraSense – AI Smart Agent

🚀 **LyraSense** is an intelligent AI-powered assistant that helps users with tasks like reminders, news updates, fun facts, and AI-based responses — all powered by FastAPI, React, and modern AI models.  

💻 **Frontend:** React (Vercel)  
⚙️ **Backend:** FastAPI (Render)  
🧠 **AI Engine:** Cohere / Groq / HuggingFace APIs  
🗂 **Database:** SQLite (for reminders and logs)

---

## 🌐 Live URLs

| Component | Platform | URL |
|------------|-----------|-----|
| **Frontend (React)** | Vercel | 🔗 [https://lyrasenselikhithajagadeesh.vercel.app](https://lyrasenselikhithajagadeesh.vercel.app) |
| **Backend (FastAPI)** | Render | 🔗 [https://lyrasense.onrender.com](https://lyrasense.onrender.com) |

---

## ✨ Features

✅ Conversational AI Assistant – Chat naturally with LyraSense  
✅ Reminders System – Create, list, and delete reminders  
✅ Fun Mode – Get fun facts when you’re bored  
✅ Web Search – Retrieves factual answers and news updates  
✅ Real-Time Integration – Connects frontend + backend via REST API  
✅ Cloud Deployed – Live globally (Render + Vercel)  
✅ Expandable – Ready for future voice input & notifications  

---

## 🧠 Tech Stack

| Layer | Technology |
|-------|-------------|
| **Frontend** | React, Axios, CSS |
| **Backend** | FastAPI, Uvicorn |
| **Database** | SQLite3 |
| **LLM Providers** | Cohere / Groq / HuggingFace |
| **Tools** | Python, Node.js, dotenv, CORS |
| **Deployment** | Vercel (frontend), Render (backend) |

---

## ⚙️ Setup Instructions (Local Development)

### 1️⃣ Clone the project
```bash
git clone https://github.com/<your-username>/lyrasense.git
cd lyrasense
```

### 2️⃣ Backend Setup
```bash
cd backend
python -m venv .venv
.venv\Scripts\activate   # (Windows)
pip install -r requirements.txt
```

Create a **.env** file:
```
COHERE_API_KEY=your_cohere_key_here
USE_PROVIDER=GROQ   # or HUGGINGFACE
```

Run backend locally:
```bash
uvicorn app:app --reload
```

Then visit:
```
http://127.0.0.1:8000/health
```

✅ Should return:
```json
{"status":"ok"}
```

---

### 3️⃣ Frontend Setup
```bash
cd frontend
npm install
```

In `src/config.js`, set your backend URL:
```js
export const API_BASE = "https://lyrasense.onrender.com";
```

Then run:
```bash
npm start
```

✅ Open [http://localhost:3000](http://localhost:3000)

---

## ☁️ Deployment Overview

### 🚀 Backend (Render)
1. Push backend folder to GitHub  
2. Go to [https://render.com](https://render.com) → New Web Service  
3. Configure:
   - **Build Command:** `pip install -r requirements.txt`
   - **Start Command:** `uvicorn app:app --host 0.0.0.0 --port 10000`
   - **Environment Variables:**  
     ```
     COHERE_API_KEY=your_key
     USE_PROVIDER=GROQ
     ```
4. Deploy → Backend live at  
   🔗 [https://lyrasense.onrender.com](https://lyrasense.onrender.com)

---

### 🚀 Frontend (Vercel)
1. Push frontend folder to GitHub  
2. Go to [https://vercel.com](https://vercel.com) → “New Project”  
3. Select frontend repo  
4. Keep defaults:
   - **Framework:** React  
   - **Build Command:** `npm run build`  
   - **Output Directory:** `build`
5. Deploy → Frontend live at  
   🔗 [https://lyrasenselikhithajagadeesh.vercel.app](https://lyrasenselikhithajagadeesh.vercel.app)

---

## 🧩 Features Demonstration (Example Commands)

| User Message | Response |
|---------------|-----------|
| `remind me to study at 6pm` | ✅ Reminder set for 'study' at 2025-11-05T18:00:00 |
| `show my reminders` | 🕒 Displays saved reminders |
| `cancel reminder 1` | 🗑 Deleted reminder #1 |
| `I feel bored` | 🎲 Returns fun fact |
| `what is artificial intelligence` | 💬 Returns AI explanation via LLM |

---

## 🛠️ Folder Structure

```
smart-agent/
├── backend/
│   ├── app.py
│   ├── reminder.py
│   ├── llm_client.py
│   ├── fun_facts.py
│   ├── news_fetcher.py
│   ├── web_search.py
│   ├── requirements.txt
│   └── reminders.db
│
└── frontend/
    ├── src/
    │   ├── App.js
    │   ├── config.js
    │   ├── App.css
    │   └── ...
    ├── public/
    ├── package.json
    └── build/
```

---

## 🧑‍💻 Author

👩‍🎓 **Shubha KC**  
  
💡 Passionate about AI, Web Development & Entrepreneurship  
🌎 Building smart solutions that empower students & developers  

---

## 🧭 Future Enhancements

- 🔔 Browser notifications for reminders  
- 🗣️ Voice interaction (Speech-to-Text + Text-to-Speech)  
- 📅 Google Calendar integration  
- 🧠 AI conversation memory  
- 💬 Real-time chat with WebSockets  

---

## 📜 License
This project is open-source under the **MIT License**.

---
Anybody fork and contribute .


---
 iam excited to collaborate and work on real agents from scratch 


 
