# 🤖 AI-Based Task Validation System

## 📌 Overview
This project is an AI-powered system that automatically validates intern task submissions by comparing them with the task description using semantic similarity.

---

## 🚀 Features
- ✅ Pre-validation (file existence, format, content length)
- 🧠 Semantic validation using Sentence Transformers
- 📊 Cosine similarity scoring
- 📂 Supports multiple file types:
  - .txt
  - .html
  - .css
  - .js
  - .ipynb
  - .docx

---

## 🏗️ System Architecture
Submission File → Pre-Validation → Semantic Validation → Result

---

## 🧠 How It Works
1. Extract text from task and submission
2. Convert text into embeddings using `all-MiniLM-L6-v2`
3. Compute cosine similarity
4. Classify result:

| Score | Result |
|------|--------|
| ≥ 0.75 | ✅ Valid |
| 0.60–0.75 | ⚠️ Partially Valid |
| < 0.60 | ❌ Invalid |

---

## 🛠️ Technologies Used
- Python
- sentence-transformers
- scikit-learn
- BeautifulSoup
- nbformat
- python-docx

---

