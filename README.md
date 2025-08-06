🔄 SMART RAG Agent
A sophisticated Retrieval-Augmented Generation (RAG) system that implements a corrective multi-stage workflow using LangGraph. This system combines document retrieval, relevance grading, query transformation, and web search to provide comprehensive and accurate responses.

Features
Smart Document Retrieval: Uses Qdrant vector store for efficient document retrieval
Document Relevance Grading: Employs gpt-4o-mini to assess document relevance
Query Transformation: Improves search results by optimizing queries when needed
Web Search Fallback: Uses Tavily API for web search when local documents aren't sufficient
Multi-Model Approach: Combines OpenAI embeddings and OpenAI llm for different tasks
Interactive UI: Built with Streamlit for easy document upload and querying
How to Run?
Clone the Repository:

git clone https://github.com/ishu3022/awesome-llm-apps.git
cd rag_tutorials/smart_rag
Install Dependencies:

pip install -r requirements.txt
Set Up API Keys: You'll need to obtain the following API keys:

OpenAI API key (for embeddings)
OpenAI API key (for gpt-4o-mini as LLM)
Tavily API key (for web search)
Qdrant Cloud Setup
Visit Qdrant Cloud
Create an account or sign in
Create a new cluster
Get your credentials:
Qdrant API Key: Found in API Keys section
Qdrant URL: Your cluster URL (format: https://xxx-xxx.aws.cloud.qdrant.io)
Run the Application:

streamlit run smartRAG_rag.py
Use the Application:

Upload documents or provide URLs
Enter your questions in the query box
View the step-by-step Smart RAG process
Get comprehensive answers
Tech Stack
LangChain: For RAG orchestration and chains
LangGraph: For workflow management
Qdrant: Vector database for document storage
gpt-4o-mini: Main language model for analysis and generation
OpenAI: For document embeddings
Tavily: For web search capabilities
Streamlit: For the user interface
