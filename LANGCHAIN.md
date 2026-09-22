
  # LangChain Roadmap

A structured roadmap for learning **LangChain** from fundamentals to production-ready LLM applications.

## 📚 Learning Path

```text
1. Introduction
      ↓
2. Model Integration
      ↓
3. Messages
      ↓
4. Prompt Templates
      ↓
5. Tools
      ↓
6. Structured Output
      ↓
7. Output Parsers
      ↓
8. Runnables / LCEL
      ↓
9. Chains
      ↓
10. Middleware
      ↓
11. Guardrails
      ↓
12. Document Loaders
      ↓
13. Text Splitters
      ↓
14. Embeddings
      ↓
15. Vector Stores
      ↓
16. Retrievers
      ↓
17. RAG
      ↓
18. Agents
      ↓
19. Agent State / Memory
      ↓
20. Evaluation
      ↓
21. LangSmith                       
                         
                         
                         
                         
                         
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
