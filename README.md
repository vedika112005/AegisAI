# 🛡️ AegisAI: Enterprise AI Governance & Audit Dashboard

**AegisAI** is a high-performance, open-source AI Governance platform designed to bridge the gap between Large Language Models (LLMs) and Enterprise Security requirements. 

It transforms "Black Box" AI into a **"Glass Box"** verifiable system, ensuring that every AI response is strictly grounded in private organizational data, logically verified, and mathematically audited to eliminate hallucinations.

---

## 🌌 Modern Enterprise Interface
AegisAI features a **Premium Dark Mode** dashboard built with glassmorphism aesthetics, designed specifically for C-suite visibility and high-performance technical auditing.

- **Glassmorphism Glass UI**: High-contrast, blurred slate aesthetics for superior readability.
- **Real-time Telemetry**: Live tracking of grounding scores, risk exposure, and pipeline progress.
- **Dynamic Governance Control**: Live sliders to adjust organizational safety thresholds without code changes.

---

## 🚀 The 10-Stage Deterministic Governance Pipeline
AegisAI routes every query through a rigorous multi-stage workflow to ensure total compliance:

1.  **🛡️ Risk Classification**: Analyzes intent to identify risk categories (Legal, HR, Finance).
2.  **🔍 Neural Retrieval**: Fetches evidence from the Knowledge Library via semantic vector search.
3.  **🧠 Intent Routing**: Powers both specific factual lookups and document-wide executive summaries.
4.  **🧩 Atomic Decomposition**: Breaks down AI responses into individual, testable factual assertions.
5.  **⚖️ Semantic Verification**: Cross-references claims against source evidence using cosine similarity.
6.  **🔬 Logic Entailment**: Uses a secondary audit model to uncover hidden assumptions or leaps in logic.
7.  **📊 Safety Quantization**: Generates a numerical **Grounding Score (%)** for every interaction.
8.  **🔄 Adaptive Regeneration**: Automatically prunes unsupported claims and forces a policy-compliant rewrite.
9.  **📜 Corporate Audit Ledger**: Immutably records the entire reasoning path to a secure database.
10. **📥 Truth Certification**: Issues downloadable **JSON Audit Certificates** for regulatory compliance.

---

## 🛠️ Key Technical Features
- **High-Performance Ingestion**: Uses local `sentence-transformers` and `PyMuPDF` for near-instant indexing of massive documents.
- **Parallel Audit Engine**: Verifies multiple factual claims simultaneously via concurrent threading.
- **Hybrid Intelligence**: Supports local inference (Ollama/Mistral) or cloud acceleration (Groq/Llama3).
- **Persistent Memory**: Full CRUD (Create/Read/Update/Delete) support for organizational knowledge documents.

---

## 💻 Installation & Quick Start

### Prerequisites
1.  **Python 3.10+** installed.
2.  **Ollama** installed (Run `ollama pull mistral` to download the reasoning engine).

### 1-Click Launch (Windows)
```cmd
# Run setup to create venv and install dependencies
setup.bat

# Launch the Dashboard and API simultaneously
run_app.bat
```

### Manual Installation
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python migrate_db.py
streamlit run app.py
```

---

## 🔌 API Integration (Headless Mode)
Integrate AegisAI's 10-stage verification loop directly into your own applications:

**Endpoint:** `POST http://localhost:8000/verify`  
**Payload Example:**
```json
{
    "query": "What are our HR data retention policies?",
    "department": "HR"
}
```

---

## ⚖️ License
Distributed under the MIT License. See `LICENSE` for more information.

---
**Powered by AegisAI Governance Engine | Verifiable. Secure. Transparent.**
