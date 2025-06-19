# Simple AI Agent

A Python-based AI assistant that can scrape websites, crawl pages, and extract data using Firecrawl tools through the Model Context Protocol (MCP). Built with LangChain, LangGraph, and powered by OpenAI's GPT-4.

## 🚀 Features

- **Web Scraping**: Scrape websites and extract data using Firecrawl
- **Interactive Chat**: Command-line interface for conversing with the AI agent
- **MCP Integration**: Uses Model Context Protocol for seamless tool communication
- **OpenAI Integration**: Powered by GPT-4 for intelligent responses
- **ReAct Agent**: Built with LangGraph's ReAct agent pattern for step-by-step reasoning
- **Async Support**: Fully asynchronous implementation for better performance

## 📋 Requirements

- Python 3.12+
- Node.js (for Firecrawl MCP server)
- OpenAI API key
- Firecrawl API key

## 🛠️ Installation

1. **Clone the repository:**

```bash
git clone https://github.com/asheint/simple-ai-agent.git
cd simple-ai-agent
```

2. **Install dependencies using uv:**

```bash
# Install uv if you haven't already
pip install uv

# Install project dependencies
uv sync
```

3. **Install Firecrawl MCP server:**

```bash
npm install -g firecrawl-mcp
```

4. **Set up environment variables:**
   Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your_openai_api_key_here
FIRECRAWL_API_KEY=your_firecrawl_api_key_here
```

## 🏃‍♂️ Usage

Run the agent:

```bash
python main.py
```

The agent will start and display available tools. You can then interact with it by typing commands. Type `exit` to quit.

### Example Interactions

- "Scrape the homepage of example.com"
- "Extract all links from https://news.ycombinator.com"
- "Crawl a website and get structured data from all pages"
- "Get the main content from a blog post"

## 📁 Project Structure

```
simple-ai-agent/
├── main.py              # Main application entry point
├── pyproject.toml       # Project dependencies and metadata
├── .env                 # Environment variables (API keys)
├── .python-version      # Python version specification (3.12)
├── .gitignore          # Git ignore rules
├── uv.lock             # Dependency lock file
└── README.md           # This file
```

## 🔧 Dependencies

- **langchain-mcp-adapters** (>=0.1.7): MCP integration for LangChain
- **langchain-openai** (>=0.3.24): OpenAI integration for LangChain
- **langgraph** (>=0.4.8): Graph-based agent framework
- **python-dotenv** (>=1.1.0): Environment variable management

## ⚙️ Configuration

The agent is configured with:

- **Model**: GPT-4 with temperature 0 for deterministic responses
- **Tools**: Firecrawl MCP tools for web scraping
- **Input Limit**: 175,000 characters per user input
- **Connection**: Stdio-based communication with MCP server

## 🏗️ Architecture

The project uses a modern Python stack:

1. **uv**: Fast Python package installer and resolver
2. **LangChain**: Framework for building LLM applications
3. **LangGraph**: Library for building stateful, multi-actor applications with LLMs
4. **MCP (Model Context Protocol)**: Protocol for connecting AI models with external tools
5. **Firecrawl**: Web scraping service with intelligent content extraction

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Run tests and ensure code quality
5. Commit your changes (`git commit -m 'Add some amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

### Development Setup

```bash
# Clone your fork
git clone https://github.com/yourusername/simple-ai-agent.git
cd simple-ai-agent

# Install development dependencies
uv sync

# Make your changes and test
python main.py
```

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🐛 Issues

Found a bug or have a feature request? Please open an issue on the [GitHub Issues](https://github.com/asheint/simple-ai-agent/issues) page.

## 🌟 Acknowledgments

- [LangChain](https://github.com/langchain-ai/langchain) for the LLM framework
- [LangGraph](https://github.com/langchain-ai/langgraph) for the agent architecture
- [Firecrawl](https://firecrawl.dev/) for web scraping capabilities
- [OpenAI](https://openai.com/) for the GPT-4 model

## 📚 Learn More

- [Model Context Protocol Documentation](https://modelcontextprotocol.io/)
- [LangChain Documentation](https://docs.langchain.com/)
- [LangGraph Documentation](https://langchain-ai.github.io/langgraph/)
- [Firecrawl Documentation](https://docs.firecrawl.dev/)

---

⭐ **Star this repository if you find it helpful!**
