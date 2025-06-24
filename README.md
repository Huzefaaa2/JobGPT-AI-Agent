# 🤖 JobGPT - AI-Powered Job Hunting Assistant

**JobGPT** is a complete end-to-end AI project built with Streamlit and OpenAI APIs to help both freshers and experienced professionals:
- 🔍 Search for relevant jobs
- 📊 Match their resume with job descriptions
- ✍️ Generate tailored cover letters
- 🎤 Simulate interviews

It is designed as a **portfolio-worthy project** for AI and software engineering aspirants, and uses **free-tier resources on Azure** or your local machine to operate fully.

---

## 🚀 Features

✅ Streamlit UI with simple interaction  
✅ Real-time job scraping using SerpAPI  
✅ Resume-JD matching with LLMs  
✅ Cover letter generation via Jinja2 templates  
✅ Interview question simulation using GPT  
✅ GitHub-ready project structure  
✅ Easily extensible and cloud-deployable  

---

## 🛠️ Tech Stack

- [Streamlit](https://streamlit.io/)
- [Python 3.9+](https://www.python.org/)
- [OpenAI API (Azure)](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/)
- [SerpAPI](https://serpapi.com/)
- Jinja2, Requests, dotenv, and more

---

## 📁 Folder Structure

```
JobGPT-AI-Agent/
│
├── jobgpt/
│   ├── job_dashboard.py         # Main UI app
│   ├── job_scraper.py           # Job fetching logic
│   ├── resume_matcher.py        # Resume vs JD comparison
│   ├── cover_letter_gen.py      # Jinja2 template rendering
│   ├── interview_bot.py         # Interview question generation
│   └── __init__.py
│
├── templates/
│   └── resume_template.jinja2   # Cover letter template
│
├── .env                         # API keys (not committed)
├── requirements.txt
└── README.md
```

---

## 🔑 Prerequisites

1. **Install Python** (≥3.9)  
   https://www.python.org/downloads/

2. **Create Accounts**
   - [Azure OpenAI](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/)
   - [SerpAPI](https://serpapi.com/)

3. **Collect API Keys**
   - `OPENAI_API_KEY`
   - `OPENAI_API_BASE`
   - `OPENAI_DEPLOYMENT_NAME`
   - `OPENAI_API_VERSION`
   - `SERPAPI_KEY`

---

## 🧪 Setup Instructions

### 1. Clone the Repo
```bash
git clone https://github.com/<your-username>/JobGPT-AI-Agent.git
cd JobGPT-AI-Agent
```

### 2. Create `.env` File
```env
OPENAI_API_KEY=your_azure_openai_key
OPENAI_API_BASE=https://your-resource.openai.azure.com/
OPENAI_API_VERSION=2024-12-01-preview
OPENAI_DEPLOYMENT_NAME=gpt-4
SERPAPI_KEY=your_serpapi_key
```

### 3. Create Virtual Environment & Install Dependencies
```bash
python -m venv venv
source venv/bin/activate   # or venv\Scripts\activate on Windows
pip install -r requirements.txt
```

### 4. Run the App
```bash
streamlit run jobgpt/job_dashboard.py
```

Open [http://localhost:8501](http://localhost:8501) in your browser.

---

## 🌐 Deployment Options

- **Streamlit Cloud**
  - Add secrets for `.env`
  - Push to GitHub and connect to Streamlit Cloud

- **Azure App Services** or **Azure Container Apps**
  - Containerize and deploy (optional advanced step)

---

## 🧠 Example Use Case

1. Enter job title/location  
2. Paste your resume  
3. Click **Find Jobs**  
4. Match and rank JD vs your resume  
5. Generate tailored cover letter  
6. Simulate interview questions  
7. Apply via the job link or manually on the company site

---

## 📦 To Do

- [ ] Add PDF resume upload and parsing
- [ ] OAuth integration for tracking applications
- [ ] Save job matches to user profile (optional DB)

---

## 🤝 Contributing

Feel free to fork, improve, and PR. This project is designed to help beginners **learn AI, APIs, and app building** in one place.

👨‍💻 Author
Huzefa Husain
🔗 LinkedIn
💻 GitHub

---

## 📄 License

MIT License
