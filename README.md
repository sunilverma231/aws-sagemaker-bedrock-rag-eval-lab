# AWS Bedrock RAG Q&A Project

This repository contains end-to-end lab notebooks and scripts for building, testing, evaluating, and securing Retrieval-Augmented Generation (RAG) applications using **Amazon Bedrock Knowledge Bases**, including integrations with LangChain, RAG evaluation (RAGAS), and Bedrock guardrails.

## Repository Content & Notebook Descriptions

| File               | Description                                                                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------------------------------|
| Task-0.ipynb       | **Environment Setup.** Installs all dependencies: AWS SDKs (boto3), LangChain, Bedrock integrations, and supporting libs.  |
| Task-1.ipynb       | **Quickstart with RetrieveAndGenerate API.** Sets up a fully-managed RAG app using Amazon Bedrock’s RetrieveAndGenerate API, validates access to an existing Knowledge Base, and demonstrates basic and custom prompting. |
| Task-2.ipynb       | **RAG with Retrieve API & LangChain.** Builds a Q&A using Bedrock's *Retrieve* API with direct similarity search, incorporates LangChain for more flexible retrieval-augmented prompt design, and connects to Anthropic Claude LLM. |
| Task-3.ipynb       | **Query Reformulation.** Shows how Bedrock’s Query Reformulation decomposes complex questions into manageable sub-queries, improving RAG response quality. Includes before/after results comparison.   |
| Task-4.ipynb       | **Evaluation with RAGAS.** Uses the RAG Assessment (RAGAS) framework to automatically evaluate RAG application answers across metrics like faithfulness, answer relevancy, context recall/precision, and correctness, exporting results to Excel. |
| Task-5.ipynb       | **Guardrails & Content Policy.** Demonstrates the deployment of guardrails using Bedrock’s RetrieveAndGenerate API to restrict responses according to custom safety, policy, and compliance rules (e.g., financial advice shielding).     |

## How To Use

1. **Clone the repo** and follow `Task-0.ipynb` to install all dependencies (ignore installation warnings as instructed).
2. Work through the notebooks in order; each one handles a logical stage in building, running, and evaluating your Amazon Bedrock RAG application.
3. Review the output and artifacts (reports, Excel files) generated for QA evaluation.
4. Use `Task-5.ipynb` to see how Bedrock guardrails prevent unsafe or non-compliant content responses in regulated scenarios.

## Highlights

- Works with Amazon Bedrock Knowledge Bases with OpenSearch serverless integration.
- Includes LangChain-based retrieval chains.
- Full RAG pipeline: ingestion, retrieval, prompting, generation, evaluation, and guardrailing.

---

**This project is great for anyone learning hands-on RAG engineering and LLM deployment on AWS with robust evaluation (RAGAS) and enterprise risk management (Guardrails).**
