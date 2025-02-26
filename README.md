Retrieval Augmented Generation Application

```mermaid
flowchart TD
    A[Data Ingestion] --> B[Splitting/Chunking]

    B --> C[Vector Embedding]

    C --> D[Vector Store]

    D <--> E[Retrievers] 

    subgraph Retrieval_chain
        direction LR
        E -- Query + Relevant documents --> F[Prompt Template]

        subgraph Chain
            direction LR
            F --> G[LLM]
        end
        H[Query] --> E
    end

    I[User] --> H

    G -- Response --> I[User]
```
