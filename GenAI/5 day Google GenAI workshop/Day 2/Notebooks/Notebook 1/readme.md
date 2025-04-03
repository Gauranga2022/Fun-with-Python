# 📘 Day 2 - Document Q&A with RAG using Chroma

This notebook is part of a Generative AI course and demonstrates how to build a Document Q&A system using **RAG (Retrieval Augmented Generation)** with **ChromaDB** and **Gemini API**.

---

## 🚀 What You’ll Learn to Do

- Understand how to overcome LLM limitations using RAG.
- Use Chroma (a vector database) to index documents.
- Retrieve relevant document snippets in response to user queries.
- Generate natural language answers using Gemini with the retrieved information.

---

## 🛠️ Step-by-Step Breakdown

### 1. **Setup**
- Install required Python libraries:
  - `google-genai` (for Gemini API)
  - `chromadb` (vector database)
- Uninstall conflicting packages (like `jupyterlab` and `kfp`).

### 2. **Authenticate with Gemini API**
- Use a Kaggle Secret to securely load your `GOOGLE_API_KEY`.
- This key gives access to Google's Gemini models via API.

### 3. **Explore Available Models**
- Use the `embedContent` API to generate vector embeddings from text.
- Choose models like `text-embedding-004` or experimental ones like `gemini-embedding-exp-03-07`.

### 4. **Document Indexing**
- Take documents (like FAQs, articles, PDFs).
- Convert them into embeddings using Gemini.
- Store them in ChromaDB with metadata for fast lookup later.

### 5. **Query Retrieval**
- When a user asks a question, turn it into an embedding.
- Use ChromaDB to find documents with similar meaning (semantic search).

### 6. **Answer Generation**
- Combine the user's question with the relevant documents.
- Send everything to Gemini to generate a final, natural language answer.

---

## 💡 Why This is Useful

- Add **custom knowledge** to LLMs (like internal documents or live info).
- Get **accurate answers** even on topics the model wasn’t trained on.
- Great for building chatbots, customer support, and search systems.

---

## 🔐 API Key Setup Tip

If you're using Kaggle, make sure you:
1. Store your key in the **Secrets** section (`GOOGLE_API_KEY`).
2. Enable it for this notebook via the Add-ons menu.

