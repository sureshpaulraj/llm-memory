# llm-memory

This repository demonstrates how to build persistent memory for LLM-based applications using Mem0, Azure AI Search, and Azure OpenAI. It includes a Jupyter notebook tutorial and a sample environment configuration.

## Overview

**llm-memory** provides a practical example of how to integrate a memory layer into your AI applications, enabling them to remember user preferences and context across sessions. This is achieved by combining:
- **Mem0**: An open-source memory layer for AI applications
- **Azure AI Search**: For storing and retrieving vector embeddings
- **Azure OpenAI**: For generating embeddings and chat completions

The included notebook walks you through setting up the environment, configuring services, and building a travel planning assistant that remembers user details.

## Features
- Store, retrieve, and search user memories using Mem0 and Azure AI Search
- Integrate Azure OpenAI for embeddings and chat completions
- Example: Travel planning assistant that remembers user preferences
- Demonstrates storing simple statements, conversations, and memories with metadata

## File Structure
- `AzureAI-Mem0-Integration.ipynb`: Main tutorial and code, with step-by-step explanations
- `.env-sample`: Template for required environment variables (do not commit your real `.env`)
- `requirements.txt`: Python dependencies
- `.gitignore`: Ensures sensitive files like `.env` are not tracked

## Getting Started

1. **Clone this repository**
   ```sh
   git clone https://github.com/sureshpaulraj/llm-memory.git
   cd llm-memory
   ```
2. **Set up environment variables**
   - Copy `.env-sample` to `.env` and fill in your Azure credentials and deployment names.
3. **Install dependencies**
   ```sh
   pip install -r requirements.txt
   ```
4. **Open the notebook**
   - Use VS Code or Jupyter to open `AzureAI-Mem0-Integration.ipynb` and follow the steps.

## Requirements
- Python 3.8+
- Azure OpenAI access (with deployed chat and embedding models)
- Azure AI Search instance

## Environment Variables
See `.env-sample` for the required variables:
- Azure OpenAI endpoint, API key, and deployment names
- Azure AI Search endpoint and admin key

**Never commit your real `.env` file.**

## Example Use Case
The notebook demonstrates a travel planning assistant that:
- Remembers user names, preferences, and travel plans
- Personalizes responses using stored memories
- Improves over time as more interactions are stored

## License
MIT

## Acknowledgments
- [Mem0](https://github.com/mem0ai/mem0)
- [Azure OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/)
- [Azure AI Search](https://learn.microsoft.com/en-us/azure/search/)
