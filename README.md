Retrieval Augmented Generation Application

## 🔄 Data Processing Flowchart

```mermaid
graph TD
    A[📥 Data Ingestion] --> B[✂️ Splitting / Chunking]
    B --> C[🔢 Embedding: Text → Vector]
    C --> D[💾 Store Vectors in Vector Store]
    D --> E{🗂️ Vector Stores}
    E --> F[Chromadb]
    E --> G[Faiss-CPU]
    E --> H[LanceDB]
    D --> I[🔍 Query]
    I --> J[🤖 Retrieval & Response]
