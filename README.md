
## 🚀 What is NLWeb?
<img src="https://github.com/RishulGupta/NLWeb-by-Microsoft/blob/d0462551e5573fe9a9796bdb214458eb03d7e03c/Screenshot%202025-07-15%20024324.png" alt="App UI" />

Recently, I explored **NLWeb**, a powerful open-source tool by Microsoft designed to simplify the integration of natural language interfaces into websites. Here's what I found and why I think it's a promising foundation for the AI-powered web.

**NLWeb** enables websites to support natural language queries natively — both for human users and AI agents. It uses Schema.org metadata (already present on over 100 million websites) and RSS-style formats to add conversational capabilities without reworking existing content structures.

At its core, NLWeb:
- Implements **open protocols** for conversational interfaces
- Supports **MCP (Model Context Protocol)** for AI agent communication
- Returns responses in **JSON using Schema.org standards**

It’s a modular framework — not a final product — encouraging developers to build upon it, just as the early Web evolved from simple servers to today’s dynamic systems.

---

## ⚙️ How It Works

NLWeb has two major components:

1. **NLWeb Protocol:** A lightweight, Schema.org-based natural language API. You ask in plain English (or other languages), it responds in structured JSON.
2. **Sample Implementation:** A reference setup that uses structured web content (like product or recipe listings) and transforms it into conversational endpoints with easy UI integration.

💡 Check out the [Life of a Chat Query](docs/life-of-a-chat-query.md) for a deeper dive.

---

## 🔄 NLWeb + MCP

NLWeb is tightly integrated with **MCP (Model Context Protocol)** — a new standard for tool-agent interaction. Every NLWeb server is also an MCP server. The core method, `ask`, is like sending an HTTP request — except you’re interacting through natural language.

> MCP is to NLWeb what HTTP is to HTML.  
> This combination powers conversational experiences that are both intelligent and structured.

---

## 🧠 AI & Platform Support

NLWeb is platform-agnostic and supports:
- **OS**: Windows, macOS, Linux
- **LLMs**: OpenAI, Gemini, Anthropic, DeepSeek, Inception
- **Vector Stores**: Milvus, Qdrant, Azure AI Search, Snowflake

It’s lightweight, scalable, and ideal for both cloud deployments and local development.

---

## 📂 What’s in the Repo?

When you clone the repo, you get:
- Core NL query service
- LLM + vector DB connectors
- Tools to ingest Schema.org JSONL / RSS
- Web frontend with a sample UI

🔧 Most real-world users can:
- Replace the sample UI with their own
- Connect to live databases (for fresh content)
- Integrate with their application stacks

---

## 📘 Documentation Highlights

- [Hello World on Your Laptop](docs/nlweb-hello-world.md)
- [Azure Setup Guide](docs/setup-azure.md)
- [Modifying Prompts](docs/nlweb-prompts.md)
- [Adding Memory](docs/nlweb-memory.md)
- [REST API Details](docs/nlweb-rest-api.md)

> AWS and GCP setup guides are coming soon.

---

## 📦 License

NLWeb is licensed under the [MIT License](LICENSE), making it free and open for modification and commercial use.

---

## 🛠️ CI/CD and Contributions

Currently, NLWeb doesn’t ship with automated CI/CD pipelines — but community contributions are welcome! Add your tools, workflows, or new features and be part of the growing ecosystem.

👉 Check [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## 👥 Community & Credits

This project is driven by a collaborative spirit. Contributions from across the open-source world are encouraged.

[![nlweb contributors](https://contrib.rocks/image?repo=microsoft/nlweb)](https://github.com/microsoft/nlweb/graphs/contributors)

For support: **NLWebSup@microsoft.com**

---

## 🧩 Final Thoughts

Exploring NLWeb gave me valuable insights into how the **AI Web** could take shape — with structured, shared protocols and easy-to-use tools for developers. It’s not just a project, but a foundational piece of a more conversational, agent-friendly internet.

> If you’re building tools that talk to people or agents — NLWeb is worth checking out.
