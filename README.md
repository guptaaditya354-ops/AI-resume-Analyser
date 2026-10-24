
# AI Resume Analyzer

An AI-powered web app that analyzes a resume and gives structured feedback: skills found, strengths, gaps, and suggestions to improve it. Built during my internship at **NathCorp**.

## Features
- Upload a resume (PDF/DOCX) and get an instant AI analysis
- Skill extraction and resume scoring
- Improvement suggestions written by an LLM (Groq API)
- Clean, responsive UI

## Tech Stack
| Layer | Tech |
|-------|------|
| Frontend | React, Vite, TypeScript, Tailwind CSS, shadcn/ui |
| Backend | Python, FastAPI |
| AI | Groq API (LLM) |

## Project Structure
```
AI-resume-Analyser/
├── backend/      # FastAPI server + resume analysis logic
├── src/          # React frontend
├── guidelines/   # UI/design guidelines
├── run_app.bat   # One-click start (Windows)
└── index.html
```

## Getting Started

### 1. Clone
```bash
git clone https://github.com/guptaaditya354-ops/AI-resume-Analyser.git
cd AI-resume-Analyser
```

### 2. Backend
```bash
cd backend
python -m venv venv
venv\Scripts\activate        # Windows
pip install -r requirements.txt
```
Create a `.env` file inside `backend/`:
```
GROQ_API_KEY=your_api_key_here
```
Start the server:
```bash
uvicorn main:app --reload --port 8000
```

### 3. Frontend
```bash
npm i
npm run dev
```
Open the URL shown in the terminal (usually http://localhost:5173).

> On Windows you can also run `run_app.bat` to start everything together.


## Future Improvements
- Job description matching (resume vs JD score)
- Support for more resume formats
- Deployment (Render / Vercel)

## Author
**Aditya Kumar Gupta**
BTech CSE (Data Science & AI/ML), Sarala Birla University, Ranchi (2027)
GitHub: [guptaaditya354-ops](https://github.com/guptaaditya354-ops)

## Credits
UI scaffold generated from a Figma export. See `ATTRIBUTIONS.md` for third-party assets.
