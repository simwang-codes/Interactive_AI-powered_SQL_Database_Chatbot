# AI-Powered SQL Chatbot (LangChain + GPT-4)

## Introduction

This project is a SQL chatbot built with LangChain and GPT-4 that allows users to ask natural language questions about a SQLite database. It automatically generates and executes SQL queries, then returns both the raw table results and a human-readable explanation.

---

## Workflow

1. **User Input**  
   ➜ Ask a question in plain English.

2. **Schema Retrieval**  
   ➜ Fetch the database schema using `LangChain SQLDatabase`.

3. **Prompt Construction**  
   ➜ Pass schema + question to GPT-4 to generate SQL.

4. **SQL Extraction**  
   ➜ Clean up and extract valid SQL using regex.

5. **Query Execution**  
   ➜ Run the SQL on `test.db` with SQLite.

6. **Final Response**  
   ➜ Return both raw table output and a GPT-4 generated natural language summary.

---

## Required Libraries

```bash
pip install langchain-core langchain-community langchain-openai openai python-dotenv pandas
```
