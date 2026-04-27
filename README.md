📄 Self-RAG Based Document QA System
A Self-Reflective Retrieval-Augmented Generation (Self-RAG) system that enables accurate question answering over documents using iterative retrieval and self-evaluation. The system improves response quality by reducing hallucinations through feedback-driven refinement.

🚀 Features
📥 PDF document ingestion and preprocessing

✂️ Text chunking for efficient retrieval

🔍 Semantic search using vector database (Qdrant)

🤖 LLM-powered answer generation using Google Gemini

🔁 Self-RAG pipeline with iterative retrieval and refinement

🧠 Stateful workflows using LangGraph

✅ Context filtering and response validation to reduce hallucinations

🛠️ Tech Stack
Backend: Python

LLM Framework: LangChain

Workflow Orchestration: LangGraph

Vector Database: Qdrant

Embeddings: FastEmbed

LLM: Google Gemini API

⚙️ How It Works
Document Upload

PDF files are loaded and processed

Chunking & Embedding

Text is split into chunks

Embeddings are generated using FastEmbed

Vector Storage

Embedded chunks are stored in Qdrant

Query Processing

User query is converted into embedding

Relevant chunks are retrieved

Self-RAG Pipeline

Initial answer is generated

System evaluates answer quality

If needed, triggers re-retrieval + refinement

Final Response

Returns improved, context-aware answer

📊 Key Highlights
Implements Self-RAG architecture instead of basic RAG

Uses feedback loops for better answer quality

Reduces hallucination via self-verification mechanisms

Supports multi-step reasoning workflows

▶️ Setup Instructions
Bash

# Clone the repository
git clone https://github.com/your-username/self-rag-project.git

# Navigate to project folder
cd self-rag-project

# Install dependencies
pip install -r requirements.txt
🔑 Environment Variables
Create a .env file and add:


GOOGLE_API_KEY=your_gemini_api_key
▶️ Run the Project
Bash

python main.py
(or run the Jupyter Notebook if applicable)

📌 Future Improvements
Add UI (React / Streamlit)

Improve re-ranking strategy

Add evaluation metrics (accuracy, relevance score)

Deploy using Docker / cloud
