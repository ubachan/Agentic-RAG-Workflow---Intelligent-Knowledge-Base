### 📂 Agentic RAG Workflow - Intelligent Knowledge Base

# 🧠 Agentic RAG Workflow

*An advanced AI Agent system that understands user intent and retrieves contextually relevant information from custom databases using Vector Search.*

## 📐 System Architecture
```mermaid
graph TD
  User((Query)) --> Hook[n8n Webhook]
  Hook --> Embed[Embedding]
  Embed --> Search{Vector Search}
  Search -- Query --> PDB[(Pinecone/MongoDB)]
  PDB -- Context --> AI[AI Model: Groq]
  AI --> Result[Synthesized Answer]
  Result --> Response[Send Response]

  style Search fill:#f9f,stroke:#333
  style PDB fill:#27272e,stroke:#fff,color:#fff
```
## 🚀 Key Features
Intent Recognition: Understands exactly what the user is asking before searching.

Vector Search: High-speed retrieval of relevant data chunks from Pinecone.

Low Latency: Optimized with Groq for near-instant AI responses.

## 🛠️ Tech Stack
- **Orchestration:**

- **Vector DB:**

- **LPU Engine:**

- **NoSQL:**
