# 📄 Resume ATS Score Analyzer

Upload a resume (PDF, DOCX or TXT) and get:

- An **ATS score** out of 100
- Section scores (formatting, keywords, experience, education, skills)
- Strengths, **specific improvements**, and suggested keywords
- Optional: paste a job description to check how well your resume matches it

Built with **Streamlit** and the **Google Gemini Flash** model.

## Project structure

```
resume-ats-analyzer/
├── app.py
├── requirements.txt
└── README.md
```

## Run locally

1. Get a free API key: https://aistudio.google.com/apikey
2. Install and run:

```bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt

export GEMINI_API_KEY="your_key_here"     # Windows PowerShell: $env:GEMINI_API_KEY="your_key_here"
streamlit run app.py
```

You can also skip the environment variable and paste the key into the app's sidebar.

To use a different Gemini model: `export GEMINI_MODEL="model-name"`.

## Push to GitHub

```bash
cd resume-ats-analyzer
git init
git add app.py requirements.txt README.md
git commit -m "Initial commit: Resume ATS analyzer"
git branch -M main
git remote add origin https://github.com/<your-username>/resume-ats-analyzer.git
git push -u origin main
```

Create the empty repo first on https://github.com/new (do not add a README there).
**Never commit your API key.**

## Deploy on Streamlit Community Cloud

1. Go to https://share.streamlit.io and sign in with GitHub.
2. Click **Create app** → choose your repo, branch `main`, main file `app.py`.
3. Open **Advanced settings → Secrets** and add:

```toml
GEMINI_API_KEY = "your_key_here"
```

4. Click **Deploy**. In a minute or two you get a public URL.

## Notes

- Scanned/image-only PDFs have no extractable text; use a text-based PDF or DOCX.
- The ATS score is an AI estimate, not the result of a real employer's ATS.
