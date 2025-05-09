
# 🤖 Autonomous Financial Health Dashboard

A smart, AI-powered dashboard that **cleans**, **analyzes**, and **explains** your monthly financials using LLMs and vector search. This tool turns raw spreadsheets into actionable business insights.

---

## 💡 What the Project Does

- ✅ **Cleans & aggregates** monthly financial CSVs
- 📊 **Calculates key KPIs**:
  - Total Sales
  - Profit
  - Burn Rate
  - Runway
- 🚨 **Detects anomalies** such as sudden profit drops or burn rate spikes
- 📝 **Summarizes each month** in natural language using an LLM
- 🧠 **Stores summaries** in a vector store (e.g. FAISS or Pinecone)
- 🔍 **Retrieves insights** using Retrieval-Augmented Generation (RAG)
- 🤖 **Answers questions** with a local or hosted LLM (e.g. Ollama, Flan-T5):
  - “Why was profit low in March?”
  - “How is our runway trending?”

---

## 🧠 Tech Stack

- **Frontend:** Streamlit
- **Backend:** Python (Pandas, Matplotlib)
- **AI Stack:** LangGraph + LLMs (Ollama or Flan-T5)
- **Vector DB:** Pinecone or FAISS
- **Deployment:** Local machine or cloud

---

## 📁 Repository Structure

```
autonomous-financial-dashboard/
│
├── app.py                    # Streamlit UI and interactions
├── financial_health.py       # Core logic: cleaning, calculating, embedding, RAG
├── data/                     # Runtime CSV uploads
├── requirements.txt          # Project dependencies
└── README.md                 # This file
```

---

## ⚙️ How to Run

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Launch the dashboard:
```bash
streamlit run app.py
```

3. Set environment variables (via `.env` or shell):
```
LLM_API_URL=
LLM_API_KEY=
```

> Works with Ollama-hosted models or any OpenAI-compatible endpoint.

---

## 📜 License

MIT License

---

## ✨ Credits

Built with ❤️ by Raane Mummaadi
