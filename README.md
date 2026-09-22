LangChain Roadmap

A structured roadmap for learning LangChain from fundamentals to
production-oriented applications.

Learning Path

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

1. Introduction

Understand what LangChain is and why it is used for LLM application
development.

Topics

What is LangChain?

Why LangChain?

LangChain ecosystem

Core packages

LLM application architecture

Basic LangChain workflow

Installing LangChain

Environment and API-key setup

Practice

Create a basic LLM application

Send a prompt to a model

Display the model response

2. Model Integration

Learn how to connect different LLM providers with LangChain.

Topics

Chat models

Model initialization

OpenAI integration

Google Gemini integration

Groq integration

Other provider integrations

Model parameters

Streaming

Model configuration

Practice

Connect multiple providers

Switch models

Compare model responses

3. Messages

Understand how conversations are represented in LangChain.

Topics

HumanMessage

AIMessage

SystemMessage

ToolMessage

Message content

Message history

Content blocks

Message metadata

Practice

Build a multi-message conversation

Inspect agent messages

Understand AI → Tool → AI execution

4. Prompt Templates

Learn how to create reusable prompts.

Topics

PromptTemplate

ChatPromptTemplate

System messages

Human messages

Variables

Partial variables

Few-shot prompts

Reusable prompt design

Practice

Create parameterized prompts

Build a reusable chatbot prompt

Create a few-shot prompt

5. Tools

Learn how LLMs interact with external functions and systems.

Topics

What is a tool?

Python functions as tools

Tool schemas

Tool arguments

Tool descriptions

Tool calling

Multiple tools

External APIs as tools

Practice

Weather tool

Calculator tool

Database/API tool

Multiple-tool agent

6. Structured Output

Learn how to make models return predictable structured data.

Topics

Structured output

Pydantic models

TypedDict

JSON schema

with_structured_output()

Validation

Structured responses

Practice

Extract customer information

Generate structured product data

Build a JSON-based response

7. Output Parsers

Learn how to process model output.

Topics

Why output parsers?

StrOutputParser

JSON output parsing

Structured output vs output parsers

Validation

Error handling

Practice

Convert model output to strings

Parse JSON responses

Validate structured responses

8. Runnables / LCEL

Learn the LangChain Runnable architecture and LCEL.

Topics

Runnable

RunnableSequence

RunnableLambda

RunnablePassthrough

RunnableParallel

Pipe operator |

invoke()

batch()

stream()

Practice

Build a pipeline:

Prompt
  ↓
Model
  ↓
Output Parser

Then build parallel and streaming workflows.

9. Chains

Understand how multiple LangChain components work together.

Topics

What is a chain?

Prompt + Model

Model + Parser

Sequential workflows

Runnable-based chains

Chain composition

Input/output flow

Practice

Build:

User Input
    ↓
Prompt
    ↓
LLM
    ↓
Parser
    ↓
Final Response

10. Middleware

Learn how to intercept and customize agent execution.

Topics

What is middleware?

Before-model middleware

After-model middleware

Tool interception

Request/response modification

Dynamic behavior

Logging

Custom middleware

Practice

Add logging middleware

Modify model requests

Implement execution controls

11. Guardrails

Learn how to control and validate LLM behavior.

Topics

Input guardrails

Output guardrails

Content validation

Policy enforcement

Tool restrictions

PII protection

Safety checks

Custom validation

Practice

Block inappropriate input

Validate model output

Restrict tool usage

12. Document Loaders

Learn how to bring external documents into LangChain.

Topics

Document concept

Document loaders

PDF loaders

Text files

CSV

JSON

Web pages

Directory loaders

Metadata

Practice

Build a document ingestion pipeline:

Files
  ↓
Document Loader
  ↓
Documents

13. Text Splitters

Learn how to divide documents into useful chunks.

Topics

Why chunking?

Chunk size

Chunk overlap

RecursiveCharacterTextSplitter

Token-based splitting

Markdown splitting

Semantic considerations

Metadata preservation

Practice

Split PDFs

Split Markdown documents

Compare chunk sizes

14. Embeddings

Learn how text is converted into vectors.

Topics

What are embeddings?

Vector representation

Embedding models

Document embeddings

Query embeddings

Similarity

Cosine similarity

Embedding dimensions

Practice

Generate embeddings

Compare similar sentences

Create document embeddings

15. Vector Stores

Learn how embeddings are stored and searched.

Topics

What is a vector store?

Chroma

FAISS

Pinecone

OpenSearch

PostgreSQL/pgvector

AWS vector database options

Similarity search

Metadata filtering

Practice

Documents
   ↓
Chunks
   ↓
Embeddings
   ↓
Vector Store

16. Retrievers

Learn how relevant information is retrieved from knowledge sources.

Topics

What is a retriever?

Vector store retriever

Similarity search

MMR

Metadata filtering

Top-K retrieval

Retriever configuration

Custom retrievers

Practice

Create a retriever from Chroma

Retrieve top-K documents

Add metadata filtering

17. RAG

Learn how to build Retrieval-Augmented Generation applications.

Topics

What is RAG?

RAG architecture

Ingestion pipeline

Retrieval pipeline

Context injection

Basic RAG

Conversational RAG

RAG evaluation

RAG optimization

Architecture

Documents
   ↓
Loader
   ↓
Splitter
   ↓
Embeddings
   ↓
Vector Store
   ↓
Retriever
   ↓
Relevant Context
   ↓
Prompt
   ↓
LLM
   ↓
Answer

Practice

Build a complete PDF Q&A application.

18. Agents

Learn how LLMs dynamically decide which tools to use.

Topics

What is an agent?

Agent vs chain

Agent loop

Tool selection

Tool calling

Agent state

create_agent()

Multiple tools

Agent execution

Agent Flow

User
 ↓
Agent
 ↓
Reason / Decide
 ↓
Tool
 ↓
Tool Result
 ↓
Agent
 ↓
Final Response

Practice

Build an agent with: - Calculator - Weather tool - Search/API tool

19. Agent State / Memory

Learn how agents maintain information during execution and across
interactions.

Topics

Agent state

Message history

Short-term state

Long-term memory concepts

State updates

Conversation history

Persistence

Checkpointing concepts

Practice

Build a conversational agent

Maintain message history

Persist agent state

20. Evaluation

Learn how to measure the quality of LLM applications.

Topics

Why evaluation?

Evaluation datasets

Reference answers

LLM-as-a-judge

Correctness

Relevance

Faithfulness

RAG evaluation

Agent evaluation

Regression testing

Practice

Create an evaluation dataset

Evaluate responses

Compare two prompts/models

Track quality over time

21. LangSmith

Learn how to observe, debug, evaluate, and monitor LangChain
applications.

Topics

LangSmith introduction

Tracing

Runs

Debugging

Prompts

Datasets

Evaluators

Experiments

Monitoring

Production observability

Practice

Enable tracing

Inspect agent execution

Trace tool calls

Create an evaluation dataset

Run experiments

Monitor application behavior

Final LangChain Architecture

After completing this roadmap, you should understand the major building
blocks:

                    LangChain
                        │
        ┌───────────────┼────────────────┐
        │               │                │
      Models          Prompts           Tools
        │               │                │
        └───────────────┼────────────────┘
                        │
                    Runnables
                        │
                     Chains
                        │
              ┌─────────┴─────────┐
              │                   │
             RAG                Agents
              │                   │
       Retrievers             Tool Calling
              │                   │
       Vector Stores         Agent State
              │                   │
        Embeddings             Memory
              │                   │
       Document Loaders       Middleware
              │                   │
       Text Splitters         Guardrails
              └─────────┬─────────┘
                        │
                    Evaluation
                        │
                    LangSmith

Recommended Project Progression

Project 1 --- Basic LLM Application

Model + Prompt + Response

Project 2 --- Structured Data Extraction

Prompt + Model + Structured Output

Project 3 --- Tool Calling Agent

Model + Tools + Agent

Project 4 --- Document Q&A

Loader + Splitter + Embeddings + Vector Store + Retriever + LLM

Project 5 --- Production RAG

RAG + Metadata + Evaluation + LangSmith

Project 6 --- Multi-Tool Agent

Agent + Multiple Tools + Middleware + Guardrails

Project 7 --- Production Agent

Agent + State + Tools + Guardrails + Evaluation + LangSmith

Suggested Order for Teaching

The roadmap follows a progression from LLM fundamentals → LangChain
components → RAG → Agents → Production.

Fundamentals
    ↓
Models
    ↓
Messages
    ↓
Prompts
    ↓
Tools
    ↓
Structured Output
    ↓
Runnables / Chains
    ↓
Middleware / Guardrails
    ↓
RAG
    ↓
Agents
    ↓
State / Memory
    ↓
Evaluation
    ↓
LangSmith
    ↓
Production-ready LLM Applications
