# "SupplyChainAgenticAI" - Food Supply Chain Resilience Agent (LangChain + LangGraph)

A multi-agent system that monitors a food supply chain, detects disruptions, and autonomously decides on replenishment actions. 
It monitors food supply chain nodes, detects  disruptions (climate shocks, stock failures), and autonomously  generates replenishment recommendations.

Free tools: LangChain + Ollama (runs LLM locally, completely free, no API key needed)



## Research Context

Built to explore agentic AI approaches to supply chain resilience — relevant to EU food security research (e.g. CARES project framework).



## Architecture

```Monitor Agent → Replenishment Agent → Report Agent```

- **Monitor Agent**: Scans all supply chain nodes, flags critical stock levels
- **Replenishment Agent**: Recommends actions (reroute, emergency restock, etc.)
- **Report Agent**: Synthesises executive summary for decision-makers



## Scenarios

- Normal operations: baseline monitoring
- Climate disruption: Farm_A supply cut 60%, system adapts



## Setup (fully free, no API key needed)

```bash
# 1. Install Ollama: https://ollama.com
ollama pull llama3.2

# 2. Install dependencies
pip install langchain langchain-ollama langgraph pandas

# 3. Run
python main.py
```



## Technologies

- LangGraph (multi-agent orchestration)
- LangChain + Ollama (local LLM, no cost)
- Python, Pandas



