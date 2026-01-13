# 🚀 AI Resume Analyzer & Job Matcher

An AI-powered web application that analyzes resumes, calculates ATS scores, recommends jobs, and suggests personalized career paths.

Built with **FastAPI** (backend) and **React + Vite + shadcn/ui** (frontend).

---

## ✨ Features

- 📄 **Resume Upload & Parsing** (PDF / DOC / DOCX)
- 🎯 **ATS Score Analysis**
- 💼 **Job Recommendations**
  - Internships & Fresher roles
  - India-focused job links (LinkedIn & Naukri)
- 📈 **Career Path Recommendations**
- 🧠 **AI-powered resume rewriting**
- 📥 **Export improved resume as PDF**

---

## 🏗️ Project Structure

```
AI-Resume-Job-Matcher/
│
├── backend/
│   ├── app/
│   │   ├── api/               # FastAPI routes
│   │   ├── services/          # ATS, jobs, AI logic
│   │   ├── datasets/
│   │   │   └── jobs.csv       # Job dataset
│   │   ├── uploads/           # Uploaded resumes
│   │   └── main.py            # FastAPI entry
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── App.tsx
│   └── vite.config.ts
│
├── .gitignore
└── README.md
```

---

## 🧑‍💻 Tech Stack

### Backend
- FastAPI
- Pandas
- Scikit-learn
- PyPDF / python-docx
- Hugging Face (API-based)

### Frontend
- React (TypeScript)
- Vite
- Tailwind CSS
- shadcn/ui
- Lucide Icons

---

## ⚙️ Backend Setup (Local)

```bash
cd backend
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Run server:

```bash
uvicorn app.main:app --reload
```

Backend runs at:

```
http://127.0.0.1:8000
```

---

## 🌐 Frontend Setup (Local)

```bash
cd frontend
npm install
npm run dev
```

Frontend runs at:

```
http://localhost:8080
```

---

## 🔌 Environment Variables

Create a `.env` file inside `backend/`:

```env
HF_API_KEY=your_huggingface_api_key
```

*(Optional – only required if using Hugging Face AI models)*

---

## 🚀 Deploy Backend on Render (FREE)

### 1️⃣ Create a New Web Service
- **Runtime:** Python
- **Root Directory:** `backend`
- **Build Command:**
```bash
pip install -r requirements.txt
```

- **Start Command:**
```bash
uvicorn app.main:app --host 0.0.0.0 --port 10000
```

---

### 2️⃣ Render Settings
- Plan: **Free**
- Auto Deploy: ✅ ON
- Region: Nearest to users

---

### 3️⃣ Render Free Tier Notes
- Repo size must be **< 500MB**
- Do NOT store large ML models locally
- Use Hugging Face via API only
- `jobs.csv` is lightweight and safe

---

## 🗂️ Jobs Dataset

Job recommendations are powered by:

```
backend/app/datasets/jobs.csv
```

Each entry includes:
- Job title
- Required skills
- Market demand
- Date posted

A scheduler updates job dates automatically.

---

## 🧹 Repository Cleanliness

This project intentionally removes:
- ❌ Lovable plugins
- ❌ Forced redirects
- ❌ Analytics injections

Ignored via `.gitignore`:
- `node_modules/`
- `__pycache__/`
- `frontend1/`
- Virtual environments
- Build artifacts

---

## 📌 Future Improvements

- 🔐 Authentication
- 📊 Resume history & versions
- 🤖 Smarter ATS scoring
- 🌍 Location-based job filters
- 📱 Mobile-first enhancements

---

## 🧠 Mission

> Built with AI to help you land your dream job.

If this project helped you, consider ⭐ starring the repo.

---

## 🤝 Contributions

Pull requests are welcome.  
Feel free to open issues for bugs or feature requests.

---

Happy building 🚀
