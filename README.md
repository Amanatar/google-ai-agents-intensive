Google AI Agents Intensive Portfolio - Aman Atar
This repository contains my capstone projects developed during the 5-Day AI Agents Intensive Course by Google and Kaggle. These projects demonstrate the use of the Google Agent Development Kit (ADK) to build autonomous, multi-agent systems.

🚀 Featured Projects
1. The Alpha Seeker (Autonomous Trading Agent)
An advanced trading system that coordinates a team of specialized agents to develop and validate investment strategies.

Architecture: Uses a SequentialAgent to manage the high-level workflow.

Parallel Processing: A ParallelAgent (QuantTeam) simultaneously fetches market data and technical indicators.

Risk Management: Implements a LoopAgent that forces the strategy to be refined until it meets specific risk criteria (Drawdown < 15%).

Cross-Agent Communication: Utilizes RemoteA2aAgent to connect the developer to a remote backtesting service.

2. Advanced Research Assistant
A multi-agent research pipeline designed to analyze complex topics from multiple perspectives.

Specialist Agents: Coordinates TechResearcher and FinanceResearcher agents.

Tool Integration: Uses Google Search for real-time data gathering.

Agent-to-Agent (A2A): Features a dedicated MathAgent exposed as an A2A service on port 8001 for financial calculations.

3. Iterative Content Creator
A content generation pipeline that mimics a professional editorial team.

Workflow: InitialWriterAgent → CriticAgent → RefinerAgent.

Iterative Refinement: Uses a LoopAgent to automatically critique and rewrite content (up to 3 iterations) until it is "APPROVED".

Custom Tools: Implements a FunctionTool (exit_loop) to programmatically stop the agentic loop.

🛠️ Technology Stack
Framework: Google Agent Development Kit (ADK).

Model: Gemini 2.5 Flash Lite.

Environment: Python, Jupyter Notebooks, Kaggle.

📋 How to Run
Install ADK:

Bash

pip install google-adk
Set API Key: Ensure your GOOGLE_API_KEY is set in your environment variables.

Run Notebooks: Open the .ipynb files in a Jupyter environment and execute the cells.

Certified on: December 18, 2025
