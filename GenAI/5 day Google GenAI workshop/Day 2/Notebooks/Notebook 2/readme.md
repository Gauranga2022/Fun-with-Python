# 🌟 Day 2 - Embeddings and Similarity Scores (with Gemini API)

This notebook is part of the Kaggle Generative AI course. It shows you how to use the **Gemini API** to compute **text embeddings** and measure **similarity** between different pieces of text.

---

## 🔍 What Are You Learning Here?

### ➤ Embeddings
- Convert text (like words, sentences, or paragraphs) into numerical vectors.
- These vectors capture the **meaning** of the text.

### ➤ Similarity Scores
- Compare how "close" two embeddings are.
- If two texts are similar, their embeddings are close = **high score**.
- If they’re different, they’re far apart = **low score**.

---

## 🛠️ What Does the Notebook Do?

### 1. **Setup**
- Installs the `google-genai` library for using Gemini API.
- Prepares the environment (removes unused packages, loads API key).

### 2. **Get Your API Key**
- Use a Kaggle secret (`GOOGLE_API_KEY`) to authenticate with Gemini API.

### 3. **Explore Embedding Models**
- You use `embedContent()` to convert text into embeddings.
- Models like `text-embedding-004` or others are used for this.

### 4. **Generate Embeddings**
- You give a list of texts (e.g. short sentences).
- The API returns a list of vectors (one for each text).

### 5. **Compare Texts**
- Use **cosine similarity** (a math formula) to check how similar two texts are.
- Print the similarity scores for different pairs of texts.

---

## 🤓 Why This is Useful

- Helps build smart search engines, chatbots, or recommendation systems.
- Great for finding **which documents are most relevant** to a user’s question.
- You can group similar content even if they use different words.

---

## 🧠 Real-Life Example

Say you have:
- "How do I reset my password?"
- "Help with forgotten login"
- "Today's weather in Paris"

The first two are similar — embedding comparison will show **high similarity**.
The last one is unrelated — it’ll get a **low score**.

---
