# Model Context Protocol (MCP): Empowering Agentic AI Interactions
**A Survey of the Model Context Protocol (MCP): A Framework for Standardized, Agentic Interactions between LLMs and External Systems**

---

## 📑 Table of Contents
- [Model Context Protocol (MCP): Empowering Agentic AI Interactions](#model-context-protocol-mcp-empowering-agentic-ai-interactions)
  - [📑 Table of Contents](#-table-of-contents)
  - [🧠 Introduction](#-introduction)
  - [📊 Comparative Analysis: MCP vs Traditional APIs](#-comparative-analysis-mcp-vs-traditional-apis)
  - [🏗️ MCP Architecture Overview](#️-mcp-architecture-overview)
  - [🧩 MCP Core Concepts](#-mcp-core-concepts)
    - [📦 Resources](#-resources)
    - [🧠 Prompts](#-prompts)
    - [🛠️ Tools](#️-tools)
    - [🎯 Sampling](#-sampling)
    - [🌐 Roots](#-roots)
    - [🔁 Transport Layer](#-transport-layer)
  - [🤖 Agentic AI \& Composability](#-agentic-ai--composability)
  - [🧭 End-to-End MCP Workflow](#-end-to-end-mcp-workflow)
 
  - [🌍 MCP in the Wild](#-mcp-in-the-wild)
  - [🧠 AI Stacks Supporting MCP](#-ai-stacks-supporting-mcp)

---

## 🧠 Introduction

The **Model Context Protocol (MCP)** provides a structured, standardized way for **Large Language Models (LLMs)** to seamlessly interact with external tools, resources, and systems—much like how APIs and Language Server Protocols revolutionized application integration.  
MCP empowers the next generation of **agentic AI** by enabling autonomous, secure, and context-rich interactions.

---


## 📊 Comparative Analysis: MCP vs Traditional APIs

| Feature                | Traditional APIs     | Model Context Protocol (MCP) |
| ---------------------- | -------------------- | ---------------------------- |
| **Tool Usage**         | Manual, bespoke code | Dynamic, standardized calls  |
| **Prompt Interaction** | Basic text-based     | Structured and context-aware |
| **Context Handling**   | Limited              | Integrated, built-in         |
| **Discovery**          | Manual               | Dynamic and introspective    |
| **Security**           | Varies widely        | Enforced mechanisms          |

---

## 🏗️ MCP Architecture Overview

<div align="center">
  <img src="assets/overview-model-context-protocol.svg" width="80%" alt="Overview of MCP Client-Server Architecture" />
  <p><em>Fig. 1: MCP Client-Server Architecture.</em></p>
</div>

---

## 🧩 MCP Core Concepts

### 📦 Resources
- **Structured External Data:** Exposes content such as text, audio, PDFs, system logs, and databases.
- **Types:**
  - **Text Resources** (e.g., JSON, source code)
  - **Binary Resources** (e.g., PDFs, videos)
- **Discovery:** Via endpoints like `resources/list` and URI templates.

---

### 🧠 Prompts
- **Reusable Templates:** For standardized LLM interactions.
- **Dynamic Context Injection:** Supports arguments and multi-step workflows.
- **Access Points:** Via `prompts/list` and `prompts/get`.

---

### 🛠️ Tools

<div align="center">
  <img src="assets/tool.png" width="75%" alt="MCP Tools" />
  <p><em>Fig. 2: Tools provide active invocation using defined JSON schemas.</em></p>
</div>

- **Executable Capabilities:** Trigger actions and external system calls.
- **Definition:** Each tool is defined with a name, description, input/output schema, and validation.
- **Invocation:** Accessed via `tools/list` and invoked using `tools/call`.

---

### 🎯 Sampling

<div align="center">
  <img src="assets/sampling.svg" width="75%" alt="MCP Sampling Flow" />
  <p><em>Fig. 3: Secure and contextual LLM completions via MCP sampling.</em></p>
</div>

- **Server-Initiated:** Sends messages to the LLM through the client.
- **Human-in-the-Loop:** Incorporates review/approval for secure execution.
- **Control Parameters:** Enables fine-tuning (temperature, token limits, etc.).

---

### 🌐 Roots

<div align="center">
  <img src="assets/root.svg" width="75%" alt="MCP Roots" />
  <p><em>Fig. 4: Roots define operational boundaries using URIs.</em></p>
</div>

- **Logical Boundaries:** Define scopes (directories, API endpoints) for resource access.
- **Multi-Context Support:** Enables composable, dynamic agent workflows.

---

### 🔁 Transport Layer

- **Real-Time Communication:** Utilizes secure HTTP/SSE channels.
- **Reliable Messaging:** Ensures structured, bidirectional interaction.

---

## 🤖 Agentic AI & Composability

MCP isn’t just a protocol—it’s a catalyst for **agentic AI**. This section outlines how MCP empowers autonomous agents to interact, collaborate, and chain tasks dynamically.

- **Dual Role Components:** MCP nodes can act as both clients and servers.
- **Dynamic Agent Chaining:** Supports complex workflows where an orchestrator agent triggers specialized sub-agents based on context.
- **Human Oversight:** Built-in review processes maintain security and reliability.

<div align="center">
  <img src="assets/mcp_composability.png" width="80%" alt="Agentic AI & Composability" />
  <p><em>Fig. X: Agentic AI enabled by MCP composability, illustrating dynamic agent chaining.</em></p>
</div>

---

## 🧭 End-to-End MCP Workflow

<div align="center">
  <img src="assets/mcp-use-case.png" width="90%" alt="MCP Workflow Example" />
  <p><em>Fig. 5: Customer Support Chatbot Workflow powered by MCP.</em></p>
</div>

**Workflow Highlights:**
1. **Capture & Send:** Client submits a structured prompt.
2. **Secure Transport:** Data is exchanged via the Transport Layer.
3. **Dynamic Invocation:** Server retrieves tools and resources as needed.
4. **Sampling & Review:** Server requests LLM completions with human oversight.
5. **Response Generation:** Outputs are returned in a clear, structured format.

---


## 🌍 MCP SERVER

| **Category**       | **Examples/Providers**                |
| ------------------ | ------------------------------------- |
| **AI & ML**        | PerplexityAI, Semantic Scholar, LMNT  |
| **Design Tools**   | Figma, Canva                          |
| **Productivity**   | ClickUp, Google Tasks, Airtable       |
| **CRM**            | HubSpot, Salesforce                   |
| **Education**      | Canvas, Blackboard                    |
| **Dev Tools**      | GitHub, Docusign, Firebase, Snowflake |
| **Mapping & Data** | Google Maps, WeatherMap               |

👉 Explore more at: [mcp.composio.dev](https://mcp.composio.dev) | [MCP GitHub Servers](https://github.com/modelcontextprotocol/servers)

---

## 🧠 AI Stacks Supporting MCP

- **LangChain:** Enables dynamic agent workflows.
- **CrewAI:** Facilitates multi-agent coordination.
- **LlamaIndex:** Supports retrieval-augmented generation.
