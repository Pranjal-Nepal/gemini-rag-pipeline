# Retrieval-Augmented Generation (RAG) with Gemini

A lightweight Retrieval-Augmented Generation (RAG) pipeline built using LangChain and Google's Gemini models (`gemini-3.5-flash-lite`). It retrieves relevant context from documents and generates grounded responses to user queries.

## 🚀 Features
- **Document Ingestion & Chunking**: Parses custom documents from the `data/` directory.
- **Semantic Retrieval**: Fetches relevant context chunks based on vector similarity.
- **Gemini Integration**: Uses Google's Gemini Flash model via `langchain-google-genai` for fast, accurate synthesis.
- **Secure Configuration**: Manages API credentials using local `.env` variables.

## 📂 Project Structure
```text
RAG/
├── data/                  # Source documents (PDFs/Text)
├── pipeline.ipynb         # Main retrieval & generation notebook
├── requirements.txt       # Project dependencies
├── .env.example           # Template for environment variables
└── README.md              # Project overview
```

## 🛠️ Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure API Key:**
   Create a `.env` file in the root directory:
   ```env
   GOOGLE_API_KEY=your_gemini_api_key_here
   ```

4. **Run the Notebook:**
   Open `pipeline.ipynb` and execute the cells sequentially.