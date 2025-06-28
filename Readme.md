## 📌 Overview
This project showcases the design and implementation of a domain-specific Legal AI Assistant, built using Dify and Ollama. It automates repetitive tasks commonly found in legal workflows, such as:

## 📄 Document review

📚 Legal precedent retrieval

⏰ Deadline tracking

✍️ Contract drafting and email summarization

📌 Citation handling

## ⚙️ Technologies Used
Dify: For managing multi-agent LLM workflows and user-facing UI integration

Ollama: For running lightweight large language models locally and privately

LangChain: Used under the hood for agent orchestration (optional but compatible)

Python: Core logic, prompt routing, API calls

Markdown/PDF Parsers: For preprocessing and tokenizing legal documents

## 🧩 Key Features
Agent Collaboration: Supports multi-agent interaction to divide and delegate legal tasks

Prompt Engineering: Optimized prompt design for legal document classification and summarization

Workflow Automation: YAML-based flow files automate sequential steps from file upload to reference retrieval

Use-Case Driven Design: Tailored for tasks such as:

Extracting legal precedents

Generating contracts

Summarizing case files and emails

## 🚀 Example Workflow
text
Copy
Edit
[1] Upload contract PDF
   ↓
[2] Automatically chunk and parse contents
   ↓
[3] Retrieve relevant case law from knowledge base
   ↓
[4] Generate summary and suggest clauses
   ↓
[5] Output markdown & send via email
## 📁 Repository Structure
···
├── app.py # Entry point for web or CLI interface
├── lawglance_main.py # Core logic for agent orchestration
├── requirements.txt # Python dependencies
├── .github/
│ └── workflows/ # (Optional) GitHub Actions or CI/CD
└── README.md # Project overview (this file)
···
---

## 📚 **Legal Coverage**

LawGlance currently supports the following laws, with plans to expand internationally:

- 📜 **The Bharatiya Nyaya Sanhita, 2023**
- 🚨 **The Bharatiya Nagarik Suraksha Sanhita, 2023**
- 🧾 **The Bharatiya Sakshya Adhiniyam, 2023**

---

## 💻 **Developer Quick Start Guide**

Ready to get started? Follow these simple steps to set up **LawGlance** on your machine:

1. **Clone the Repository** 🌀
    ```bash
    git clone https://github.com/lawglance/lawglance.git
    ```

2. **Install uv** 📂

    First, let’s install uv and set up our Python project and environment
    
    MacOS/Linux:
      ``` bash 
      curl -LsSf https://astral.sh/uv/install.sh | sh
      ```

    Windows:

      ``` bash 
      powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
      ```
    Make sure to restart your terminal afterwards to ensure that the uv command gets picked up.

3. **Install Dependencies** 📦
    ```bash
    uv sync
    ```

4. **Set Your OpenAI API Key** 🔑

   Open `.env` and add your OpenAI API key:
      ```bash
      OPENAI_API_KEY=your-api-key-here
      ```

5. **Run the Application** 🚀
    ```bash
    uv run streamlit run app.py
    ```

6. **Access the App** 🌐  
    Open your browser and visit:  
    ```bash
    http://127.0.0.1:8501
    ```

---

## 🔧 **Tools & Technologies**

| 💡 **Technology**  | 🔍 **Description**                            |
|--------------------|-----------------------------------------------|
| **LangChain**       | Framework for building language models       |
| **ChromaDB**        | Vector database for RAG implementation       |
| **Django**          | High-level Python web framework for robust apps|
| **OpenAI API**      | Powering natural language understanding      |

---

