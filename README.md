# 📚 GRE Vocabulary Quiz — Web & Streamlit Versions

Lightweight GRE vocabulary quiz tools for fast, practical vocab practice.  
Includes both a client-side HTML version and a Python Streamlit version.

---

## 🌐 1. HTML Version (`gre_quiz.html`)

A simple, standalone browser-only GRE vocab quiz.  
No server, no installation — just double-click and start studying.

### ✨ Features
- 4-choice multiple-choice quiz  
- Load your own wordlist (Excel → copy → paste)  
- Randomized questions & shuffled answer options  
- Score tracking  
- Auto-generated *Wrong Answer Notes*  
- One-click note export (review / Anki import)  
- 100% client-side (runs locally)

### 🚀 How to Use
1. Open **`gre_quiz.html`** in Chrome or Safari.  
2. Copy your wordlist from Excel:  
   - Column A = **word**  
   - Column B = **meaning**  
3. Paste into the input box.  
4. Click **Load Words** → choose number of questions.  
5. Start the quiz.  
6. Copy your **wrong-answer notes** at the end for review.

---

## 🐍 2. Streamlit Version (`gre_quiz_app.py`)

A more interactive version built with Streamlit.  
Supports Excel upload and persistent session-based question flow.

### ✨ Features
- Upload your own `.xlsx` file  
- Expected columns:  
  - **word** (string)  
  - **meaning** (string)  
- Random MCQ generation (4 choices)  
- Session-based state (current question, answer tracking)  
- “Next question” without resetting the app  
- Consistent UI even on page refresh  
- Fully local — no backend/server required

### ▶️ Run Locally
```bash
pip install streamlit pandas
streamlit run gre_quiz_app.py
