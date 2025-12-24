# Microsoft Agent Framework Tutorial

A hands-on tutorial exploring Microsoft's new Agent Framework and Azure AI Agent Service for building enterprise-grade AI agents.

## What is the Microsoft Agent Framework?

The **Microsoft Agent Framework** is Microsoft's unified, open-source SDK for building, orchestrating, and deploying sophisticated AI agents. It brings together the best of Semantic Kernel and AutoGen into a production-ready framework that integrates seamlessly with Azure AI Foundry and Azure AI Agent Service.

### Key Capabilities:

- **Cloud-Hosted Agents**: Deploy and manage agents on Azure with enterprise-grade security, durability, and observability
- **Built-in Tools**: File Search, Code Interpreter, Bing Grounding, Azure AI Search, and custom function calling
- **Multi-Agent Orchestration**: Connect agents, create workflows, and implement handoff patterns
- **Enterprise Features**: Role-based access control, content safety, data persistence, and OpenTelemetry integration
- **Model Flexibility**: Support for Azure OpenAI, OpenAI, and other model providers

## Learning Objectives

This tutorial covers the Azure AI Agent Service through three progressive notebooks:

1. **[Agent Service Basics](1-agent-service-basics.ipynb)** - Core concepts including agent creation, threads, conversations, and function calling
2. **[Agent Tools & Capabilities](2-agent-tools-capabilities.ipynb)** - Built-in tools like File Search, Code Interpreter, Bing Grounding, and streaming responses
3. **[Multi-Agent Orchestration](3-multi-agent-orchestration.ipynb)** - Connected agents, sequential workflows, handoff systems, and human-in-the-loop patterns

## Prerequisites

### Azure Requirements
- Azure subscription with access to Azure AI Foundry
- Deployed Azure AI Foundry Project
- Deployed language model (e.g., gpt-4o, gpt-4.1)

### Optional Resources (for specific tutorials)
- Bing Search resource (for web grounding)
- Azure AI Search resource (for enterprise search)

### Local Requirements
- Python 3.10 or higher
- Azure CLI installed and configured (`az login`)

## Setup

### Installation

1. Create a Python virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install required packages:
```bash
pip install azure-ai-projects azure-identity python-dotenv aiohttp
```

3. Configure your environment by creating a `.env` file with your Azure credentials (see `.env.example` for the template).

### Authentication

The tutorials use `DefaultAzureCredential` for authentication. Make sure you're logged into Azure CLI:
```bash
az login
```

Or set up a service principal with appropriate permissions.

## Environment Variables

Create a `.env` file in the `agent-framework` directory with the following:

```env
# Azure AI Foundry Project
PROJECT_ENDPOINT=https://<your-project>.services.ai.azure.com

# Model deployment name (used for agents)
MODEL_DEPLOYMENT_NAME=gpt-4o

# Optional: Bing Search connection (for grounding)
BING_CONNECTION_NAME=your-bing-connection

# Optional: Azure AI Search connection
AZURE_AI_SEARCH_CONNECTION_NAME=your-search-connection
```

## Resources

- [Azure AI Agent Service Documentation](https://learn.microsoft.com/en-us/azure/ai-foundry/agents/)
- [Azure AI Agents Python SDK](https://learn.microsoft.com/en-us/python/api/overview/azure/ai-agents-readme)
- [Microsoft Agent Framework GitHub](https://github.com/microsoft/agent-framework)
- [Azure AI Foundry Samples](https://github.com/azure-ai-foundry/foundry-samples)
- [Build Your First Agent Workshop](https://microsoft.github.io/build-your-first-agent-with-azure-ai-agent-service-workshop/)

## Comparison with Semantic Kernel

| Feature | Semantic Kernel | Azure AI Agent Service |
|---------|----------------|----------------------|
| Hosting | Self-hosted | Cloud-hosted on Azure |
| State Management | Manual | Built-in persistence |
| Tools | Plugin-based | Built-in + Custom |
| Multi-Agent | Orchestration patterns | Connected agents |
| Enterprise Features | Via integration | Native Azure features |
| Best For | Flexibility, self-hosted | Enterprise, managed |

Both frameworks can work together - Semantic Kernel can be used alongside Azure AI Agent Service for complex orchestration scenarios.

## Getting Started

Start with the first notebook and progress through the series to build your understanding of the Microsoft Agent Framework and Azure AI Agent Service.

Happy building! 🚀
