# GCMP_2024A
## Global Capital Markets Platform (GCMP)
Overview
The Global Capital Markets Platform (GCMP) is an AI-driven multi-agent system designed to streamline and optimize processes across global financial markets. The platform leverages a central controller LLM (LLaMA 3.3 70B) and specialized smaller fine-tuned models to execute specific tasks, such as risk assessment, trade execution, compliance monitoring, and market data analysis.

This project visualizes and implements a structured, modular workflow to enable real-time task orchestration, decision-making, and interaction with external tools and systems.

# Architecture
The architecture is based on multi-agent collaboration, where the Central Controller LLM oversees task delegation, aggregates results, and delivers outputs. The system comprises the following key components:

# 1. Central Controller LLM
The Central Controller LLM serves as the brain of the system.
It receives user requests, breaks them into subtasks, delegates tasks to specialized models, and aggregates the final output.
It ensures seamless inter-agent communication and task optimization.
2. Specialized LLMs
These smaller fine-tuned models perform domain-specific tasks efficiently:

# Risk Assessment Model: Fetches and evaluates market data for credit risk and exposure analysis.
Trade Execution Model: Makes trade decisions and interacts with execution engines for order routing.
Regulatory Compliance Model: Monitors processes for adherence to financial regulations.
Market Data Analysis Model: Analyzes historical and real-time market data to provide insights.
3. Tools
The platform integrates with external tools to execute its tasks:

# Market Data APIs: Provides live and historical financial data.
# Execution Engines: Interfaces for trade routing and clearing.
# Compliance Monitoring Systems: Tools for regulatory oversight and anomaly detection.
# Quantitative Libraries: Supports quantitative modeling and analytics.

# Workflow
The platform follows a modular and parallel workflow, as represented in the diagram:

# User Request:

The process begins with a request for market analysis, risk evaluation, or trade execution.
Central Controller LLM:

Breaks down the user request into manageable subtasks.
Delegates tasks to specialized LLM agents.
Specialized LLMs:

Each specialized model completes its assigned task:
Risk Assessment → Fetches data via Market Data APIs.
Trade Execution → Executes trades via Execution Engines.
Compliance Monitoring → Flags anomalies using Compliance Monitoring Systems.
Market Analysis → Provides insights using Quantitative Libraries.
Tool Integration:

# Specialized models interact with external tools to fetch, process, or execute data.
Result Aggregation:

# The Central Controller LLM aggregates results from all specialized models.
Output Delivery:

# The aggregated output is delivered to the user in the desired format.

## Diagram
Below is a visual representation of the GCMP workflow:




# Central Controller LLM: The orchestrator of the entire workflow.
Specialized LLMs: Perform risk assessment, trade execution, compliance monitoring, and data analysis.
Tools: Facilitate integration with market data providers, trade systems, and monitoring tools.
# Features
Scalability: Modular design allows easy scaling of specialized models and tools.
Efficiency: Fine-tuned smaller models optimize resource usage while maintaining accuracy.
Real-Time Execution: Enables dynamic market monitoring, analysis, and decision-making.
Compliance-Driven: Integrates robust compliance tools for regulatory adherence.
