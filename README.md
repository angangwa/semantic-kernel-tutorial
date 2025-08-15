# Semantic Kernel Tutorial

A hands-on tutorial exploring Microsoft's Semantic Kernel SDK for building AI agents and applications.

## Learning Objectives

This tutorial covers the fundamentals of Semantic Kernel through three progressive notebooks:

1. **[Semantic Kernel Basics](1-semantic-kernel-basics.ipynb)** - Core concepts including chat completion, agents, plugins, and function calling
2. **[Advanced Agent Features](2-semantic-kernel-advanced.ipynb)** - Streaming responses, structured outputs, reasoning models, and intermediate steps
3. **[Multi-Agent Orchestration](3-semantic-kernel-orchestration.ipynb)** - Group chat patterns, concurrent processing, handoff systems, and human-in-the-loop workflows

## Setup

### Prerequisites
- Python 3.10 or higher
- Azure OpenAI or OpenAI API access

### Installation

1. Create a Python virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install Semantic Kernel:
```bash
pip install semantic-kernel==1.35.2 python-dotenv
```

3. Configure your environment by creating a `.env` file with your API credentials (see notebook examples).

## Important Note

Semantic Kernel is under active development with rapid feature evolution. The Agent Framework transitioned to GA in Q1 2025, but some features demonstrated in the orchestration notebook may be experimental and subject to change. Microsoft uses experimental attributes to signal evolving APIs before stabilization.

## Getting Started

Start with the first notebook and progress through the series to build your understanding of AI agent development with Semantic Kernel.