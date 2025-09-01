# AI Resume Agent 📝🤖
An AI-powered resume tailoring agent that takes a Job Description (JD) + Resume and generates a tailored, ATS-friendly resume using LLMs.

---

## 🚀 Features
- Parse Job Descriptions and Resumes (PDF/Word/Text)
- Gap Analysis between JD and Resume
- AI-powered Resume Generation
- Export to DOCX (PDF support planned)
- Agentic design (Parser → Analyzer → Generator → Exporter)

---

## ⚙️ Tech Stack
- **Backend**: FastAPI (Python 3.11)
- **LLMs**: OpenAI GPT, Gemini, DeepSeek (pluggable)
- **Parsing**: PyPDF2, python-docx
- **Export**: python-docx
- **Containerization**: Docker

---

## 📦 Installation (Local)

```bash
git clone <repo-url>
cd ai-resume-agent
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env   # Add your API keys
uvicorn app.main:app --reload
