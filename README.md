# Government-Scheme-retrival-system-using-LLMs

[Link to new full code version](https://github.com/Misty033/GovScheme_RAG)

### Project Overview
This project leverages the power of Large Language Models (LLMs) and vector databases to build a smart system that retrive eligible government schemes based on user inputs. It also provides detailed information about specific schemes on request. The first scrape government websites, then automates the process of extracting scheme details, structuring data, and semantically searching through it using LLMs and embeddings.

### Problem Statement
Government websites host a wide range of schemes targeted at different citizen groups. However, navigating and finding the right scheme can be overwhelming due to:
1. Poorly organized data
2. Scattered information across multiple sites
3. Complex eligibility criteria
4. Lack of personalized search tools
5. As a result, citizens often miss out on benefits they are eligible for.

###  Solution
1. This project solves the problem by building a LLM-powered recommendation system that:
2. Scrapes official government websites for scheme data.
3. Extracts and processes the content into a structured format (JSON).
4. Chunks the data and generates vector embeddings using an embedding model.
5. Stores the embeddings in a vector database for fast similarity search.
6. Uses a LLM (like OpenAI GPT or similar) to:
7. Recommend eligible schemes based on user input (e.g., age, occupation, income).
8. Answer user queries about specific government schemes in natural language.

### Procedure
1. Web Scraping
Crawl URLs from official government portals hosting schemes.
Scrape textual content using libraries like requests, BeautifulSoup, or Selenium.

2. Text Extraction and Cleaning
Extract relevant scheme details (e.g., name, objective, eligibility, benefits).
Clean and normalize the content.

3. JSON Conversion
Structure the extracted data into JSON format for uniformity.

4. Text Chunking
Split long scheme descriptions into manageable chunks suitable for embedding.

5. Embedding Generation
Use models like OpenAI's text-embedding-ada-002 or HuggingFace models to convert text chunks into high-dimensional vectors.

6. Vector Database Creation
Store the embeddings in a vector store.

7. Query System with LLM
Accept user details (e.g., age, occupation, income, region).
Match user data with scheme eligibility criteria via semantic search.
Use an LLM to interpret, refine, and explain results.
Answer natural language questions about specific schemes.
    
### Tech Stack
1. Python
2. BeautifulSoup  – Web scraping
3. n8n – LLM orchestration
4. Google gemini – Embeddings + LLM
5. Pinecone – Vector store
6. Streamlit – UI for interaction

### Future Work
1. Add multilingual support for regional audiences.
2. Integrate real-time scheme updates.
3. Scheme Validity Alerts and Updates for User

## This project is a prototype version and had been deployed successfully in May, 2025.
