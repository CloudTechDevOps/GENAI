                         LangChain
                             │
          ┌──────────────────┼──────────────────┐
          │                  │                  │
        Models             Prompts            Tools
          │                  │                  │
          └──────────────────┼──────────────────┘
                             │
                         Runnables
                             │
                           Chains
                             │
                ┌────────────┴────────────┐
                │                         │
               RAG                     Agents
                │                         │
          Retrievers                 Tool Calling
                │                         │
        Vector Stores                Agent State
                │                         │
          Embeddings                    Memory
                │                         │
       Document Loaders              Middleware
                │                         │
        Text Splitters               Guardrails
                │                         │
                └────────────┬────────────┘
                             │
                         Evaluation
                             │
                         LangSmith
