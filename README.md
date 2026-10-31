# Autonomous Multi-Agent Systems: Google ADK & The Alpha Seeker

<div align="center">

[![CI Verified](https://github.com/Amanatar/google-ai-agents-intensive/actions/workflows/ci-verify.yml/badge.svg)](https://github.com/Amanatar/google-ai-agents-intensive/actions)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Google ADK](https://img.shields.io/badge/Google-Agent_Development_Kit-4285F4?logo=google&logoColor=white)](https://github.com/google/agent-development-kit)
[![Gemini](https://img.shields.io/badge/Gemini-2.0_Flash-8E75C2?logo=google-gemini&logoColor=white)](https://deepmind.google/technologies/gemini/)

</div>

Autonomous multi-agent architectures built for the **Google AI Agents Intensive** capstone competition on Kaggle, coordinating specialized LLM agents for quantitative financial research and automated market signal validation.

---

## Systems Architecture

### 1. The Alpha Seeker: Autonomous Trading Agent (`03-alpha-seeker-trading-agent/`)
- **Multi-Agent Coordination:** Implements sequential, parallel, and feedback-loop agent topologies using the **Google Agent Development Kit (ADK)**:
  - *Macro Analyst Agent:* Ingests financial headlines, interest rate decisions, and broad market sentiment.
  - *Technical Valuation Agent:* Queries real-time price feeds via `yfinance`, calculating momentum, moving average crosses, and volatility regime shifts.
  - *Risk Governor Agent:* Enforces mandatory capital preservation rules (maximum drawdown limit < 15%, position sizing constraints).
  - *Synthesis Agent:* Aggregates multi-agent votes into a final risk-adjusted portfolio recommendation.

### 2. Advanced Multi-Turn Research Assistant (`02-advanced-research-assistant/`)
- **Automated Evidence Synthesizer:** Multi-agent pipeline equipped with web retrieval, cross-source verification, and structured synthesis.

---

## Setup & Running

```bash
git clone https://github.com/Amanatar/google-ai-agents-intensive.git
cd google-ai-agents-intensive

python -m venv .venv
# Activate virtual environment:
# Linux/macOS: source .venv/bin/activate
# Windows: .venv\Scripts\activate

pip install -r requirements.txt
```

Launch Jupyter or execute notebooks directly:
```bash
jupyter notebook 03-alpha-seeker-trading-agent/the-alpha-seeker-autonomous-trading-agent-adk.ipynb
```

---

## License
MIT License. Copyright 2026 Aman Atar.
