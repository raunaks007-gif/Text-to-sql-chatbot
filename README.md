# 🤖 Text-to-SQL AI Assistant

An AI-powered application that enables users to interact with relational databases using natural language instead of SQL. The system leverages Large Language Models (LLMs) to translate user queries into executable SQL statements, retrieve results from a MySQL database, and generate human-readable responses.

---

## 📌 Overview

Business users often need insights from databases but lack SQL expertise. This project bridges that gap by combining **LangChain**, **Google Gemini 2.0 Flash**, and **MySQL** to create an intelligent assistant capable of understanding natural language questions and converting them into accurate SQL queries.

The assistant dynamically understands the database schema, executes generated SQL queries, and presents the results in an easy-to-understand format.

---

## 🚀 Features

- 💬 Natural Language to SQL conversion
- 🗄️ MySQL database integration
- 🧠 Google Gemini 2.0 Flash for SQL generation
- 🔗 LangChain-based prompt pipeline
- 📊 Automatic SQL execution and result retrieval
- 📝 Human-readable response generation
- 🛡️ Query evaluation using RAGAS
- 🔍 LLM-based safety and quality assessment
- ⚡ Schema-aware dynamic prompt engineering

---

## 🏗️ Tech Stack

| Category | Technologies |
|----------|--------------|
| Programming Language | Python |
| LLM | Google Gemini 2.0 Flash |
| Framework | LangChain |
| Database | MySQL |
| Evaluation | RAGAS |
| LLM Evaluator | Groq (Gemma2-9B) |
| Notebook | Jupyter Notebook |

---

## 📂 Project Structure

```
Text-to-SQL-AI-Assistant/
│
├── Agentic Approach.ipynb
├── Gemini Chatbot.ipynb
├── Gemini Chatbot (including RAGAS).ipynb
├── customers.csv
├── products.csv
├── sales_order.csv
├── regions.csv
├── 2017_budgets.csv
├── README.md
└── requirements.txt
```

---

## ⚙️ Workflow

1. User enters a natural language question.
2. LangChain retrieves the database schema.
3. Gemini generates the SQL query.
4. SQL executes on the MySQL database.
5. Retrieved data is converted into a natural language response.
6. RAGAS evaluates query correctness and response quality.

---

## 📊 Example Queries

```
Show total sales for each region.

Which product generated the highest revenue?

List the top 10 customers by sales.

What was the total budget for 2017?

Show monthly sales trend.
```

---

## 📈 Evaluation

The project incorporates **RAGAS** for automated evaluation of generated responses using:

- Context Precision
- Rubric Score
- SQL correctness
- Response quality
- Safety evaluation
- Hallucination detection

An additional LLM (Gemma2-9B via Groq) is used as an evaluator to assess response quality against predefined rubrics.

---

## 🎯 Applications

- Business Intelligence
- Sales Analytics
- Financial Reporting
- Retail Analytics
- Customer Analytics
- Healthcare Data Analysis
- Enterprise Database Querying

---

## 🔮 Future Improvements

- Streamlit Web Application
- Role-based Authentication
- Database Support (PostgreSQL, SQL Server, Oracle)
- SQL Error Self-Correction
- Data Visualization Dashboard
- Multi-Agent Architecture
