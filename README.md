# 🍽️ Restaurant Review RAG Chatbot

An AI-powered Restaurant Review Assistant built using **Retrieval-Augmented Generation (RAG)**. Instead of relying solely on a language model's knowledge, the chatbot retrieves relevant restaurant reviews from a vector database and uses them as context to generate accurate, context-aware responses.

---

## 🚀 Features

- 🔍 Semantic search over restaurant reviews
- 💬 Natural language question answering
- 🧠 Retrieval-Augmented Generation (RAG)
- 📄 CSV-based knowledge base
- ⚡ Fast vector search with ChromaDB
- 🤖 Local LLM and embeddings using Ollama

---

## 🛠️ Tech Stack

- Python
- Pandas
- LangChain
- Ollama
- ChromaDB

---

## 📂 Project Structure

```text
Restaurant-RAG/
│
├── reviews.csv          # Restaurant review dataset
├── main.py              # Main application
├── requirements.txt     # Python dependencies
├── chroma_db/           # Vector database
└── README.md
```

---

## ⚙️ How It Works

1. Load restaurant reviews from a CSV file.
2. Convert each review into vector embeddings using Ollama.
3. Store the embeddings in ChromaDB.
4. When a user asks a question:
   - Retrieve the most relevant reviews.
   - Pass those reviews to the LLM as context.
   - Generate a context-aware answer.

### Pipeline

```text
Restaurant Reviews (CSV)
          │
          ▼
    Load with Pandas
          │
          ▼
 Generate Embeddings
     (Ollama)
          │
          ▼
 Store in ChromaDB
          │
          ▼
     User Question
          │
          ▼
 Semantic Retrieval
          │
          ▼
      Relevant Reviews
          │
          ▼
   LLM Generates Answer
```

---

## 💻 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Restaurant-RAG.git
cd Restaurant-RAG
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate it.

Windows:

```powershell
.\venv\Scripts\Activate.ps1
```

macOS/Linux:

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

Make sure Ollama is running and the required model has been downloaded.

Then run:

```bash
python main.py
```

---

## 📌 Example Questions

- What do customers think about the pizza?
- Which dishes receive the best reviews?
- Are customers happy with the service?
- Is the restaurant family-friendly?
- What complaints appear most frequently?

---

## 📖 What I Learned

This project helped me understand:

- Retrieval-Augmented Generation (RAG)
- Vector embeddings
- Semantic search
- Vector databases (ChromaDB)
- LangChain pipelines
- Prompt engineering
- Local LLM deployment with Ollama

---

## 🔮 Future Improvements

- Web interface using Flask or React
- Multiple restaurant support
- PDF and menu ingestion
- Conversation memory
- Streaming responses
- Deployment on cloud
- Hybrid search (keyword + semantic)
- User authentication

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

---

## 📜 License

This project is licensed under the MIT License.
