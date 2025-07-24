
# 🧠 Intelligent Query Resolution Workflow (n8n)

This repository contains an advanced n8n workflow that intelligently resolves user queries by combining structured data lookup, multi-LLM response generation, and AI-based evaluation. It’s designed for scalable, multi-source question answering using spreadsheets, PDFs, and large language models.

---

## 📌 Features

- ✅ Excel-based Q&A lookup for fast answers
- 🤖 Multi-LLM querying (e.g., GPT-4, Claude, Gemini)
- ⚖️ LLM Judge node to evaluate and select best response
- 📄 PDF parsing and embedding generation
- 🔁 Feedback loop to update Excel with new answers
- 🧩 Modular design for easy customization

---

## 🧰 Technologies Used

- [n8n](https://n8n.io/) for workflow orchestration
- Google Sheets or Excel for structured Q&A
- OpenAI / other LLM APIs for dynamic responses
- LangChain or custom logic for judging and scoring
- PDF parsing via HTTP Request or custom nodes

---

## 📂 Files Included

- `multi-doc-answer-pipeline.json` – Main n8n workflow file



## 🚀 How to Use

### 1. Import Workflow into n8n
- Open your n8n editor
- Click ☰ → **Import Workflow**
- Select `multi-doc-answer-pipeline.json`

### 2. Configure Credentials
- Set up API credentials for OpenAI or other LLMs
- Connect your Google Sheets or Excel node
- Add PDF source or upload logic if needed

### 3. Run the Workflow
- Trigger manually or via webhook
- Input a query and watch the pipeline resolve it intelligently

---

## 🧪 Workflow Logic

1. **Excel Lookup** – Checks if the query exists in the Q&A sheet
2. **LLM Cascade** – Sends query to multiple LLMs if not found
3. **LLM Judge** – Evaluates responses and selects the best one
4. **Answer Delivery** – Returns the final answer to the user
5. **Feedback Loop** – Optionally logs new answers back to Excel

---

## 📦 Optional Enhancements

- Add GitHub webhook for auto-import
- Use GitHub Actions for CI/CD
- Integrate vector search with Milvus or Pinecone
- Build a frontend for user query input

---

## 📄 License

MIT License. Feel free to fork, modify, and contribute.

---

## 🙌 Contributions

Pull requests welcome! If you have ideas to improve the workflow or add new LLM integrations, let’s collaborate.


