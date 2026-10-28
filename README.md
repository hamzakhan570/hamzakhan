# hamzakhan
# AI Research Assistant 🔬

A beginner-friendly AI research assistant built with Python,
Streamlit, Google's Gemini Flash API, and PyPDF.

## Features

- Ask questions about research topics
- Upload PDF, TXT, and Markdown documents
- Generate summaries and key findings
- Adapt explanations to beginner, intermediate, and advanced users
- Create a learning roadmap
- Download reports as Markdown files

## Requirements

- Python 3.10 or later
- A Gemini API key from https://aistudio.google.com/

## Run locally

1. Clone or download this repository.
2. Install dependencies:

   pip install -r requirements.txt

3. Create `.streamlit/secrets.toml` and add:

   GEMINI_API_KEY = "your-api-key-here"

4. Start the app:

   streamlit run app.py

5. Open the local URL shown in the terminal.

Never upload your API key or `secrets.toml` to GitHub.

## Deploy on Streamlit Community Cloud

1. Upload `app.py`, `requirements.txt`, and `README.md` to GitHub.
2. Visit https://share.streamlit.io/
3. Sign in with GitHub and select Create app.
4. Select your repository, branch, and `app.py`.
5. Open Advanced settings and enter your secret:

   GEMINI_API_KEY = "your-api-key-here"

6. Click Deploy.

## Limitations

- PDF extraction works best with text-based PDFs.
- Scanned PDFs may require OCR.
- The app does not automatically browse the web.
- AI-generated claims and references should be verified.
