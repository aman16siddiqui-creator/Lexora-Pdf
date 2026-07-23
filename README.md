📘 **Project:**

Intermediate RAG System Using Pinecone Vector Database

📌 **Course:**

Artificial Intelligence / NLP / Applied LLM Systems

📅 **Level:**

Intermediate

🎯 **Objective:**

🔹 Design and implement a Retrieval-Augmented Generation (RAG) system that:

🔹 Accepts a PDF document as input

🔹 Extracts and processes text from the document

🔹 Generates embeddings

🔹 Stores embeddings in Pinecone vector database

🔹 Retrieves relevant context based on user query

🔹 Generates accurate answers strictly from the PDF content

🔹 The system must prevent hallucination and provide traceable answers.

🏗️ **System Architecture Requirements:**

Implement the following pipeline:

PDF Upload ➡️ Text Extraction ➡️ Text Chunking ➡️ Embedding Generation ➡️ Pinecone Vector Indexing ➡️ Semantic Retrieval ➡️ LLM Response Generation ➡️ Answer with Source Reference

🧰 **Required Technologies:**

🔹 Python

🔹 Streamlit or FastAPI (for interface)

🔹 LangChain (optional but recommended)

🔹 Sentence Transformer or equivalent embedding model

🔹 Pinecone Vector Database

🔹 LLM API (Groq / OpenAI / Open-source model)

🧲 **Vector Database Requirement:**

Must use:

🔹 Pinecone

The implementation must demonstrate:

🔹 Index creation

🔹 Namespace usage

🔹 Upserting vectors

🔹 Querying vectors

🔹 Managing metadata

📋 Functional Requirements

The system must:

1️⃣ PDF Upload

🔹 Accept at least one PDF file

🔹 Support files up to 20 MB

2️⃣ Text Processing

🔹 Extract text from PDF

🔹 Remove unnecessary formatting artifacts

🔹 Apply intelligent text chunking

3️⃣ Embeddings

🔹 Convert chunks into vector embeddings

🔹 Store embeddings in Pinecone

🔹 Include metadata:

🔹 Page number

🔹 Document name

🔹 Chunk ID

4️⃣ Retrieval

🔹 Retrieve top-k relevant chunks

🔹 Use cosine similarity

🔹 Allow adjustable similarity threshold

5️⃣ Answer Generation

🔹 Use retrieved context to generate answers

🔹 Restrict answers strictly to provided context

🔹 If context is insufficient, return: "The answer is not available in the provided document."

6️⃣ Source Attribution

Display:

🔹 Page number

🔹 Relevant excerpt

🔹 Similarity score

📊 **Non-Functional Requirements:**

🔹 Clean modular architecture

🔹 Separation of concerns (loader, retriever, generator, etc.)

🔹 Environment variable handling for API keys

Error handling for:

🔹 Invalid PDF

🔹 Empty queries

🔹 Pinecone connection failure

📈 **Intermediate-Level Enhancements (Mandatory):**

🔹 Multi-document support

🔹 Query history (session memory)

🔹 Adjustable chunk size from UI

🔹 Adjustable top-k retrieval

🔹 Metadata filtering (e.g., filter by page)

🔹 Confidence scoring display

🔹 Logging user queries

📊 **Evaluation Rubric:**

           Criteria	                          Weight
           
🔹 System Architecture Design	                 20%

🔹 Pinecone Integration	                       20%

🔹 Retrieval Accuracy                        	 20%

🔹 Hallucination Prevention	                   15%

🔹 Code Structure & Modularity	               15%

🔹 Documentation & Report	                     10%
