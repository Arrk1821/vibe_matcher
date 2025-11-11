# 🎨 Vibe Matcher — AI Fashion Recommender

This project builds a lightweight AI system that understands “vibes” to recommend fashion items matching a user’s mood or style.  
Using **free TF-IDF embeddings** and **cosine similarity**, the system takes short natural-language vibe queries — like _“energetic urban chic”_ or _“cozy hygge sweater”_ — and returns the **top-3 most similar fashion products**.

---

## 🧠 Why AI at Nexora
I built this project to explore how AI can make product discovery more human. Instead of keyword matching, it interprets the *feeling* behind a query — showing how simple NLP techniques can create personalized, intuitive recommendations.  
Nexora’s vision of connecting AI with creativity inspired this approach to blend human intuition with intelligent data systems.

---

## ⚙️ Tech Stack
- Python (Jupyter Notebook)
- **Pandas**, **NumPy**, **scikit-learn**
- TF-IDF for embeddings (free offline alternative)
- Cosine similarity for ranking products

---

## 🚀 Features
- Works fully offline — no API key or billing needed  
- Matches vibe queries to top-3 fashion products  
- Displays similarity scores for transparency  
- Includes fallback handling for low-similarity cases  
- Logs latency and evaluates query accuracy

---

## 📊 Evaluation
| Metric | Result |
|--------|---------|
| Queries Tested | 3 (“energetic urban chic”, “cozy hygge sweater”, “evening glam slip dress”) |
| Avg Latency | < 5 ms |
| Accuracy Metric | Top-3 ranked by cosine similarity |
| Threshold | 0.3 (fallback trigger) |

---

## 🧩 Reflection & Improvements
1️⃣ Replaced paid API embeddings with free TF-IDF vectors — fast, lightweight, and no billing required.  
2️⃣ System returns top-3 fashion products for any “vibe” query using cosine similarity.  
3️⃣ Handled edge cases — fallback message if similarity < 0.3.  
4️⃣ Achieved average query latency under 5 ms — responsive for small datasets.  
5️⃣ Future upgrades: integrate OpenAI embeddings, Pinecone for large-scale vector search, and personalized recommendations.

---

## 🏁 How to Run
1. Open `vibe_matcher_notebook.ipynb` in **Jupyter** or **Google Colab**  
2. Run all cells in order  
3. Try your own vibe queries (e.g. `"minimal streetwear"`)

---

## 📈 Future Upgrades
- Replace TF-IDF with OpenAI `text-embedding-3-small` for real semantic understanding  
- Add Pinecone / FAISS for scalable vector search  
- Build a simple web demo with Gradio or Streamlit

---

⭐ **Author:** Arrk Raj  
📅 **Project Type:** AI Mini Recommender (Assignment — Nexora)
