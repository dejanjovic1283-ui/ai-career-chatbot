# 🤖 AI Career Chatbot Pro

An AI-powered career assistant that reads a resume from PDF, optionally uses a target job description, and answers career-related questions through a chat interface.

## 🚀 Features

- Upload resume in PDF format
- Extract text automatically
- Optional job description support
- Chat interface for resume and career questions
- Embedding-based retrieval
- FAISS vector search
- LLM-generated answers
- Resume-job fit analysis
- Missing skills detection
- Profile summary rewrite

## ⚙️ Tech Stack

- Python
- Streamlit
- pdfplumber
- sentence-transformers
- FAISS
- OpenAI API

## 🧠 How it works

1. The app extracts text from a PDF resume.
2. It splits the text into chunks.
3. It creates embeddings for retrieval.
4. It stores embeddings in a FAISS vector index.
5. When the user asks a question, the app retrieves the most relevant chunks.
6. It sends the retrieved context and the user question to the LLM.
7. The LLM returns a contextual, career-focused answer.

## ▶️ Run locally

```bash
pip install -r requirements.txt
streamlit run app.py

🔐 Secrets

Create a file:
.streamlit/secrets.toml
and add:
OPENAI_API_KEY = "your_api_key_here"

💬 Example questions

- What are the strongest parts of my resume?
- What skills are missing for this job?
- Am I a good fit for this position?
- Rewrite my profile summary to better match this job.

📌 Future Improvements

- Persistent chat history
- Cover letter generator
- Resume rewrite mode
- Multi-file support
- Cloud deployment

👨‍💻 Author
- Dejan Jović