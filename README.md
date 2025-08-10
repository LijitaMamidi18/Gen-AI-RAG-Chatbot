
---

# ** Q&A System**

**An End-to-End Mistral + LangChain Project for an E-Learning Platform**

The goal of the project is to **reduce the repetitive workload** on the human support staff by providing a **Streamlit-based AI assistant** that can instantly answer student queries from the  **FAQ dataset**.

---

## **Key Features**
* **End-to-End AI Workflow** – From data ingestion to embedding generation, vector storage, retrieval, and LLM-based answer generation.
* **User-Friendly UI** – Built with **Streamlit** for smooth, interactive question answering.
* **Scalable Knowledge Base** – Students can query the bot anytime, reducing manual intervention.
* **Fast and Relevant Responses** – Answers are returned in seconds with contextual accuracy.

---


## **Technical Workflow**

1. **Data Collection**
2. **Embedding Generation** – Convert each FAQ into dense vector representations using **HuggingFace Instructor Embeddings**.
3. **Vector Storage** – Store embeddings in a **FAISS vector index** for quick retrieval.
4. **Question Input** – Students enter questions through the Streamlit UI.
5. **Context Retrieval** – FAISS searches for the most relevant FAQ entries based on semantic similarity.
6. **Answer Generation** – LangChain passes the retrieved context to **Mistral**, which formulates a human-like answer.
7. **Response Delivery** – The generated answer is displayed instantly in the web interface.



## **Project Structure**

| File                      | Description                                                                                  |
| ------------------------- | -------------------------------------------------------------------------------------------- |
| **`main.py`**             | The main Streamlit app that handles the front-end and integrates with backend logic.         |
| **`langchain_helper.py`** | Contains LangChain pipeline logic for embedding, retrieval, and LLM calls.                   |
| **`requirements.txt`**    | List of Python dependencies for reproducibility.                                             |
| **`.env`**                | Stores sensitive credentials (Google API key).                                               |
| **`faiss_index/`**        | Auto-generated directory containing the FAISS vector database after knowledge base creation. |


