# 🤖 AutoML Code Assistant with LLMs

A full-stack AI-powered assistant that transforms your **dataset + ML task prompt** into a **runnable, ready-to-download machine learning project** — complete with Python code, outputs, and documentation.

---

## 🔍 Quick Stats

- 🧠 **50+ prompts tested** across classification, regression, EDA, and time series tasks  
- 📂 **10+ datasets parsed** (.csv/.xlsx) with header extraction  
- ⚙️ **90%+ prompt-to-pipeline success rate** in internal testing  
- ⏱️ **~5 seconds** average response time from LLM to code generation  
- 📦 Generates **7+ ready-to-run artifacts** per session (`.py`, `.txt`, `.png`, `.md`)  
- 🧪 Zero manual edits required for **>85%** of outputs

---

## 🎬 Demo Video

▶️ Watch the full walkthrough here:  
**[🔗 YouTube Demo](https://youtu.be/X7v3r7xscCE)**
---
Built using:
- ⚛️ React + Material UI (frontend)
- 🐍 Python (ML engine with LLM)
- 🚀 Node.js + Express (backend API)
- 🧠 [OpenRouter](https://openrouter.ai/) + Mixtral LLM

---

## 🧠 What It Does

1. **Upload your dataset** (.csv/.xlsx)
2. **Enter a natural language prompt**  
   _E.g., "Build a classification model to predict customer churn"_
3. The app:
   - Extracts dataset headers
   - Sends everything to an LLM (Mixtral via OpenRouter)
   - Generates clean, working Python ML code
   - Executes the code (plots, stats, etc.)
4. **Download** a full ZIP:
   - `dataset.csv`
   - `step_1_train_model.py`, `step_2_plot_accuracy.py`...
   - `output_step_X.png` or `.txt`
   - `pipeline.py` (chained runnable version)
   - `README.md` and `requirements.txt`

---

## 🚀 Example Use Cases

| Prompt Example | Result |
|----------------|--------|
| Build a classifier for churn prediction | sklearn model, accuracy score |
| Perform exploratory data analysis | head(), describe(), correlation plot |
| Plot sales over time | matplotlib time series |
| Train a regression model for housing prices | regression + MSE output |

---

## 🛠️ Technologies Used

### Frontend
- React
- Material-UI

### Backend
- Node.js + Express
- Python (LLM code engine)
- `child_process` for running Python
- `multer` for file upload
- `archiver` for ZIP generation

### LLM
- OpenRouter API
- Mixtral-8x7B-Instruct

---

## 📦 Example ZIP Contents

```

📁 session\_1721253282042/
├── dataset.csv
├── step\_1\_train\_model.py
├── output\_step\_1.txt
├── pipeline.py
├── requirements.txt
└── README.md

```

> All outputs are automatically generated and bundled. You can run the full pipeline in one go using `pipeline.py`.

---

## 🔐 API Keys

You’ll need an OpenRouter API key (free-tier available):

```

OPENAI\_API\_KEY=sk-xxxxxxx

```

Get it from: https://openrouter.ai/

---

## ✨ Future Features (Ideas)

- Switch between GPT-4, Mixtral, Claude, etc.
- Visual output gallery
- Code execution sandbox (security)
- Collaborative sessions with history
- HuggingFace / Render deployment

---

## 🙌 Credits

Built with ❤️ by Preya Shah — AI, full-stack, and ML enthusiast.
