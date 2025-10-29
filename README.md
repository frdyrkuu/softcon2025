# Building the Future of Work: NVIDIA's Agentic AI Platform for Organizational Transformation

**Speaker:** Hariharan Suresh  
**Event:** SOFTCON 2025  
**Topic:** NVIDIA’s Agentic AI Platform and its role in transforming organizational workflows.

---

## Overview

This session introduced **NVIDIA's framework for Agentic AI**, detailing how organizations can **build, deploy, and scale intelligent AI agents** using NVIDIA’s multi-layered technology stack.  

The presentation described the **building blocks of Agentic AI**, composed of:
- **AI Infrastructure:** GPU, CPU, and Networking layers.
- **NVIDIA NIM**
- **NVIDIA NeMo**
- **AI Blueprints** – including pre-built examples like Research Assistant and Customer Service Agents.

---

## NVIDIA NIM (NVIDIA Inference Microservice)

A key focus of the presentation was **NVIDIA NIM**, a system designed for running **pre-trained, optimized AI models up to 5X faster**.  

### Key Characteristics:
- Supports **community, partner, and NVIDIA models** across domains such as Speech, Computer Vision, Language, and RAG.  
- Built to be **cloud-native**, operating on **Kubernetes and CUDA**.  
- Integrates **NVIDIA TensorRT-LLM** for high-performance inference.  
- Optimized for **single-GPU, multi-GPU, and multi-node environments**.

---

## Llama Nemotron: Advanced Agentic Reasoning Models

The session highlighted **NVIDIA Llama Nemotron**, which delivers **advanced agentic reasoning** through **enterprise-grade, production-ready models**.  

### Model Tiers:
| Model | Description | Deployment Target |
|--------|--------------|-------------------|
| **Llama Nemotron Nano** | Highest accuracy on PC and edge | PC / Edge |
| **Llama Nemotron Super** | Best accuracy with highest throughput | Data Center GPU |
| **Llama Nemotron Ultra** | Maximum agentic accuracy | Multi-GPU Data Center Servers |

These models excel in **complex reasoning** and **instruction following**, optimized for enterprise applications.

### Model Development Process:
1. **Distillation** – Initial model compression and knowledge transfer.  
2. **Supervised Fine-Tuning (SFT)** – Enhanced with NVIDIA-curated reasoning skills.  
3. **Reinforcement Learning (RL)** – Alignment with human preferences.

---

## NVIDIA NeMo Agent Toolkit

The **NeMo Agent Toolkit** is presented as an **open-source framework** for building **enterprise-ready agentic systems**.  

### Key Functions:
- **Profiling & Optimizations**
- **Evaluation & Observability**
- **Agent Interconnect** – leveraging a **Config Builder** and **Tool Registry**

---

## AI-Q (Pronounced “IQ”) NVIDIA Blueprint

The **AI-Q Blueprint** is an **open-source framework** that integrates **Nemotron reasoning models** with **AI agents, data, and tools** for tasks such as research and reporting.  

### Core Capabilities:
- Upload and connect **custom data sources**.  
- **Synthesize hours of material in minutes**.  
- Designed for **multi-modal, large-scale data processing**.

### Main Components:
| Component | Function |
|------------|-----------|
| **Llama Nemotron** | Boosts AI agents with reasoning skills – "#1 Open Reasoning Models" |
| **NeMo Retriever** | Connects AI agents to data for fast, accurate, multi-modal retrieval |
| **NeMo Agent Toolkit** | Connects, evaluates, and optimizes agentic systems while identifying bottlenecks |

---

## From Prototype to Production

The session concludes by showing the **path from prototype to production** using NVIDIA’s ecosystem:

1. **Experiment and build** at [build.nvidia.com](https://build.nvidia.com)  
2. **Scale across multiple clouds** for production deployment.

---

## Key Takeaways

- NVIDIA’s Agentic AI platform enables **end-to-end development of intelligent agents** using open, optimized models.  
- **Llama Nemotron** provides powerful reasoning capabilities across deployment scales.  
- The **NeMo Agent Toolkit** and **AI-Q Blueprint** empower organizations to integrate, evaluate, and scale AI systems efficiently.  
- NVIDIA’s ecosystem bridges the gap from **prototype experimentation** to **enterprise-grade production**.

---

# Beyond Chatbots: Unlocking the Power of Agentic AI with watsonx Orchestrate

**Speakers:** Joyson Barrago & Tristan Mahinay  
**Event:** SOFTCON 2025  
**Topic:** Exploring the shift from traditional chatbots to Agentic AI using IBM’s watsonx Orchestrate.

---

## Overview

This session introduces **Agentic AI** as a significant evolution beyond traditional AI models and chatbots.  
The agenda covers:
- The Agentic Shift  
- Agentic AI Concepts  
- The watsonx Orchestrate  
- Use-case Demonstration

---

## The Agentic Shift

The presentation positions Agentic AI as the **third stage** in the evolution of artificial intelligence:

| Stage | Description |
|--------|--------------|
| **Models** | AI that can **generate** for you |
| **Assistants** | AI that can **chat** for you |
| **Agents** | AI that can **do** for you |

Unlike Assistants—described as **feed-forward systems**—Agents are powered by a **think–act–observe loop**, allowing them to **adapt to real-time data** within a feedback system.

---

## Core Components of AI Agents

Agentic AI is defined by three primary components:

1. **Perception**  
   The agent *senses* its environment through inputs such as:
   - User prompts  
   - Website data  
   - Database information  

2. **Planning & Reasoning**  
   Acts as the *brain* of the agent by:
   - Breaking down large tasks  
   - Finding optimal solutions  
   - Deciding appropriate actions  

3. **Action**  
   The agent executes plans using various tools, such as:
   - Web browsers  
   - Applications or APIs  

A diagram titled **“What are AI Agents”** illustrates this ecosystem — showing an **AI Agent** capable of:
- **Task Delegation**  
- **Autonomous Actions**  
- Interaction with **Tools**, **Memory**, and **Protocols** (e.g., MCP)  
- Involvement of a **Human in the Loop**

---

## Traditional Generative AI vs. Agentic AI

The session contrasts traditional assistants with agentic systems through an example on **personal loan queries**:

| Approach | Description | Example Query | Result |
|-----------|--------------|----------------|--------|
| **Traditional Gen AI** | Uses an LLM and knowledge base to provide direct responses. | “What are common types of personal loans?” | Lists secured and unsecured loans. |
| **Agentic AI** | Uses orchestrated agents for complex, data-driven reasoning. | “Which personal loan options offer the best interest rates and repayment flexibility for individuals with a credit score below 650?” | Coordinates multiple agents (Product Research, Credit Risk, Compliance) to generate a synthesized, specific response (e.g., “Credit union loans with 8–12% APR”). |

---

## Key Concepts and Enabling Technologies

### Tools (Function Calling)
The ability of an AI system to **invoke external functions, APIs, or services** beyond its model parameters.  
Example: A model calls a **Flight API** to answer a question about an upcoming flight.

---

### Vector Store / Knowledgebases
A **specialized database** that stores and manages data as **vectors** to represent semantic meaning.  
This allows the AI to:
- Retrieve **contextually relevant information**, not just keyword matches.  
- **Augment model responses** with factual and up-to-date data.

---

### Model Context Protocol (MCP)
An **open standard** that simplifies how AI models **connect and interact** with external data sources and tools.  
It serves as a **universal adapter** to solve the “M × N” integration problem—removing the need for custom connections for each tool.

---

## Agentic AI Patterns

The session introduces four common **Agentic AI design patterns**, each representing a unique reasoning and execution approach:

| Pattern | Description |
|----------|--------------|
| **Reflect** | Processes a user query via an LLM that refines the request into a more precise **Reflected Response**. |
| **ReAct** | Combines **Reasoning** and **Acting**, where an agent uses tools and interacts with its environment to achieve goals. |
| **Tool Pattern** | Uses **Tool Calling** to access a **Tool Database**, then synthesizes results to form the final response. |
| **Multi-agent Pattern** | A **Manager Agent** coordinates multiple **Sub-agents** (e.g., News Agent, Subreddit Agent, Mirror Agent) to produce a comprehensive or “scenic” response. |

---

## Key Takeaways

- **Agentic AI** marks a shift from chat-based systems to autonomous, action-driven intelligence.  
- It integrates **perception, reasoning, and action** to operate flexibly within real-world environments.  
- **watsonx Orchestrate** demonstrates how multi-agent collaboration and orchestration can deliver more intelligent, contextual, and data-backed results.  
- Core technologies like **function calling**, **vector stores**, and **MCP** make these systems modular, adaptable, and extensible.

---

# Agents of Change: Building Intelligent Software That Works for You

**Speaker:** Allan Mangune  
**Event:** SOFTCON 2025  
**Theme:** Agentic Ignition – Powering the Future of Software  
**Topic:** Understanding the anatomy of AI agents and their real-world application.

---

## Overview

This session defines the **core components of an AI Agent** and demonstrates how they can be applied in intelligent, automated workflows.  
The presentation explores how modern agents combine reasoning, memory, perception, and action within a continuous feedback loop to create **AI-driven software systems**.

---

## Anatomy of an AI Agent

The **Anatomy of an AI Agent** is presented through five essential components:

| Component | Description |
|------------|--------------|
| **Brain (Reasoning Engine)** | The central system responsible for interpreting data and making decisions. |
| **Memory** | Stores previous information, enabling context-aware reasoning and continuity. |
| **Perception (APIs, Events)** | Allows the agent to sense and receive input from external sources or events. |
| **Action (Tools, Services)** | Executes operations and interacts with tools or applications to fulfill tasks. |
| **Feedback Loop** | Continuously evaluates results and refines future actions. |

---

## Demonstrations

The session features a **multi-stage demo** showcasing the reasoning and visualization capabilities of AI agents.

### Demo Stage 3 – Reasoning
This stage demonstrates **natural language reasoning** applied to structured financial data.  
An example prompt:  
> “Is this stock beautiful? Explain why.”

Here, the agent uses **ChatGPT** to analyze data points such as:
- Revenue  
- Margins  
- Debt  
- Returns  

The model then produces a **clear verdict and plain-English explanation**, showing how agents interpret complex data logically.

---

### Demo Stage 4 – Visualization
In this stage, the agent:
- **Converts data into visuals and metrics automatically**  
- **Eliminates manual reporting and chart creation**  

This automation highlights how AI can streamline data interpretation and business intelligence workflows.

---

## Demo Reflection

The session summarizes the demo process under the concept of **Agent Orchestration**, following the pattern:

plan → act → evaluate


This framework is adaptable across multiple domains, including:
- Human Resources (HR)  
- Finance  
- Analytics  

---

## Key Message

The presentation concludes with a forward-looking message:

> “The future isn't just AI-powered — it's AI-driven.”  
> “Start small, automate one process, and let software think for you.”

---

## Key Takeaways

- AI Agents are built from five interconnected components: **Reasoning, Memory, Perception, Action, and Feedback.**  
- The **plan–act–evaluate** pattern defines agent orchestration across industries.  
- Automated reasoning and visualization can replace traditional manual workflows.  
- The shift toward **AI-driven software** encourages organizations to begin with small, focused automation efforts.

---


