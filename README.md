# 🧠 Psychology RAG Chatbot

An intelligent **Retrieval-Augmented Generation (RAG)** chatbot built using:

- Python
- LangChain
- FAISS Vector Database
- HuggingFace Embeddings
- Groq LLM API
- PDF Knowledge Base

This chatbot reads psychology PDF documents and answers user questions based only on the uploaded document.

---

# 🚀 Features

✅ PDF document reading  
✅ Smart chunking for better retrieval  
✅ FAISS persistent memory  
✅ Fast semantic search  
✅ Groq Llama 3.1 responses  
✅ Accurate document-based answers  
✅ Streamlit UI ready

---

# 📁 Project Structure

```bash
project/
│── app.py
│── requirements.txt
│── Psychology_Complete_Short_Guide.pdf
│── faiss_memory/
│── rag_vector_db/
│── README.md
⚙️ Installation
1️⃣ Clone Project
git clone <your-repo-url>
cd project
2️⃣ Create Virtual Environment
python -m venv venv
3️⃣ Activate Environment
Windows
venv\\Scripts\\activate
Mac/Linux
source venv/bin/activate
4️⃣ Install Requirements
pip install -r requirements.txt
🔑 Setup API Key

Replace:

groq_api_key="YOUR_GROQ_API_KEY"

Get key from:

Groq

▶️ Run Project
streamlit run app.py
🧠 How It Works
Step 1: Load PDF

Reads psychology PDF using:

PyPDFLoader()
Step 2: Split Into Chunks

Uses:

chunk_size = 350
chunk_overlap = 50
Step 3: Convert To Embeddings

Using:

sentence-transformers all-MiniLM-L6-v2

Step 4: Store In FAISS

Persistent local vector database:

faiss_memory/
Step 5: User Query

When user asks question:

Convert query → embedding
Search top relevant chunks
Send context to LLM
Step 6: AI Response

Powered by:

Groq + Llama 3.1 8B Instant

📌 Example Questions
What is psychology?
Explain anxiety disorder
What is growth mindset?
How memory works?
Explain dark psychology
⚡ Recommended Embedding Model

Use this for fast local run:

sentence-transformers/all-MiniLM-L6-v2
🛠 Tech Stack
Tool	Use
Python	Backend
LangChain	RAG pipeline
FAISS	Vector DB
Groq	Fast LLM
Streamlit	UI
HuggingFace	Embeddings
🔥 Future Upgrades
Voice chatbot
Chat history memory
Login system
Multi PDF upload
Mood detector
Therapist UI
Cloud deploy
👨‍⚕️ Disclaimer

This app is educational only. It is not a replacement for licensed mental health professionals.
