# AI Agent Tutorials

Hands-on tutorials for building AI agents using Microsoft's agent technologies.

## Tutorial Series

This repository contains two tutorial series covering different approaches to building AI agents:

### 1. Semantic Kernel Tutorial (Self-Hosted)

The Semantic Kernel tutorials cover Microsoft's open-source SDK for building AI agents that you host and manage yourself.

**Best for**: Maximum flexibility, self-hosted solutions, custom orchestration patterns

**Notebooks**:
1. **[Semantic Kernel Basics](1-semantic-kernel-basics.ipynb)** - Core concepts including chat completion, agents, plugins, and function calling
2. **[Advanced Agent Features](2-semantic-kernel-advanced.ipynb)** - Streaming responses, structured outputs, reasoning models, and intermediate steps
3. **[Multi-Agent Orchestration](3-semantic-kernel-orchestration.ipynb)** - Group chat patterns, concurrent processing, handoff systems, and human-in-the-loop workflows

**Setup**:
```bash
pip install semantic-kernel==1.35.2 python-dotenv
```

For a more thorough workshop, see: https://github.com/Azure-Samples/semantic-kernel-workshop/tree/main.

---

### 2. Microsoft Agent Framework Tutorial (Cloud-Hosted)

The **[Microsoft Agent Framework](agent-framework/)** tutorials cover Azure AI Agent Service - Microsoft's cloud-hosted platform for building and deploying enterprise-grade AI agents.

**Best for**: Enterprise deployments, managed infrastructure, built-in tools and persistence

**Notebooks**:
1. **[Agent Service Basics](agent-framework/1-agent-service-basics.ipynb)** - Creating agents, threads, conversations, and function calling
2. **[Agent Tools & Capabilities](agent-framework/2-agent-tools-capabilities.ipynb)** - File Search, Code Interpreter, Bing Grounding, and streaming
3. **[Multi-Agent Orchestration](agent-framework/3-multi-agent-orchestration.ipynb)** - Connected agents, sequential workflows, handoffs, and human-in-the-loop

**Setup**:
```bash
pip install azure-ai-projects azure-identity python-dotenv
```

**Key Features**:
- Cloud-hosted agents with persistent threads
- Built-in tools: File Search, Code Interpreter, Bing Grounding, Azure AI Search
- Enterprise security and compliance
- Multi-agent orchestration patterns

See the [Agent Framework README](agent-framework/README.md) for detailed setup instructions.

---

## Comparison

| Feature | Semantic Kernel | Azure AI Agent Service |
|---------|----------------|----------------------|
| **Hosting** | Self-hosted | Cloud-hosted on Azure |
| **State Management** | Manual | Built-in persistence |
| **Tools** | Plugin-based | Built-in + Custom |
| **Multi-Agent** | Orchestration patterns | Connected agents |
| **Enterprise Features** | Via integration | Native Azure features |
| **Best For** | Flexibility, self-hosted | Enterprise, managed |

Both frameworks can work together - Semantic Kernel can be used alongside Azure AI Agent Service for complex orchestration scenarios.

## Prerequisites

- Python 3.10 or higher
- Azure OpenAI or OpenAI API access (for Semantic Kernel)
- Azure subscription with Azure AI Foundry (for Agent Framework)

## Getting Started

1. **New to AI agents?** Start with the Semantic Kernel Basics notebook
2. **Building for enterprise?** Check out the Agent Framework tutorials
3. **Already familiar with Semantic Kernel?** Explore the Agent Framework for cloud-hosted capabilities

## Important Note

Both Semantic Kernel and Azure AI Agent Service are under active development with rapid feature evolution. Microsoft uses experimental attributes to signal evolving APIs before stabilization.

## Resources

- [Semantic Kernel Documentation](https://learn.microsoft.com/en-us/semantic-kernel/)
- [Azure AI Agent Service Documentation](https://learn.microsoft.com/en-us/azure/ai-foundry/agents/)
- [Microsoft Agent Framework GitHub](https://github.com/microsoft/agent-framework)
- [Azure AI Foundry Portal](https://ai.azure.com)
