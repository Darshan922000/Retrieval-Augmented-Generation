Retrieval Augmented Generation Application

```mermaid
flowchart TD
    A[Data Ingestion] --> B[Splitting/Chunking]
    B --> C[Embedding (Text -> Vector)]
    C --> D[Vector Store (Store Vectors)]

    D --> E[LLMs]
    E --> F[Prompt Template]
    F --> G[Chains (Combine LLMs and Prompt Template)]
    G --> H[Retrievers]
    H --> I[Retrieval Chain (Retrievers + Chains)]
    I --> J[User Query]
    J --> K[Passes through Retrieval Chain]
    K --> L[Final Response Generation]
```

