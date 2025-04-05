# 💬 Chat with PDF using Gemini

This Streamlit application allows users to **upload PDF files and interact with them conversationally** using Google's **Gemini Pro** model. The app utilizes **LangChain**, **FAISS**, and **Gemini AI embeddings** to process and understand PDF documents, enabling users to ask questions and receive intelligent, context-aware answers.

---

## 🚀 Features

- 📄 Upload and process multiple PDF files
- 🧠 Chunk large texts into manageable parts using LangChain
- 📌 Store document chunks as embeddings using FAISS
- 🤖 Ask natural language questions about your documents
- ✅ Get accurate answers using Google Gemini Pro
- 🔒 Secure API key usage via environment variables

---

## 🛠️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/Shivan5h/Chat-With-Multiple-PDF.git
cd chat-with-pdf-gemini
```

### 2. Create and activate a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔐 Setup API Key

Create a `.env` file in the project root and add your Google API key:

```
GOOGLE_API_KEY=your_google_api_key_here
```

---

## 🏃 Usage

```bash
streamlit run app.py
```

- Use the **sidebar** to upload one or more PDF files.
- Click on **Submit & Process** to extract and embed the documents.
- Ask questions in the main input bar.
- Get instant, accurate responses based on your uploaded PDFs.

---

## 🧹 Tech Stack

- **Streamlit** - Web Interface
- **LangChain** - Text processing and chaining logic
- **FAISS** - Vector storage and retrieval
- **Google Generative AI (Gemini Pro)** - Question Answering & Embeddings
- **PyPDF2** - PDF text extraction
- **dotenv** - Secure API key management

---

## 📁 Project Structure

```
├── app.py                  # Main Streamlit application
├── requirements.txt        # List of dependencies
├── .env                    # API key file (not pushed to Git)
└── faiss_index/            # Saved vector store (generated at runtime)
```

---

## 📌 Notes

- Make sure the `.env` file is not pushed to GitHub.
- You need access to Google Generative AI API and permissions to use the Gemini Pro model.
- Ensure the FAISS index is saved only after processing the documents.

---

## 📬 Feedback & Contributions

Feel free to fork this repository, create issues, or submit PRs. Contributions are welcome!

---
