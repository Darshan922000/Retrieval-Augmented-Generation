Retrieval Augmented Generation Application

```mermaid
flowchart TD
    A[Data Ingestion] --> B[Splitting/Chunking]

    B --> C[Vector Embedding]

    C --> D[Vector Store]

    D <--> E[Retrievers] <-- H[Query] <-- I[User]

    E --> F[Prompt Template]

    F --> G[LLM]

    G --> J[Response] --> I[User]
```
