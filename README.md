# customer_support_autonomous_agent
AI-powered customer support agent with intent routing, Cosmos DB order lookup, FAQ handling, Azure OpenAI responses, and a Streamlit dashboard.
# Customer Support Agent

An AI-powered customer support agent that classifies user queries, retrieves relevant support data, and generates natural responses. The project includes a FastAPI backend and a Streamlit dashboard for interactive demos.

## Highlights

- Intent-based routing for support queries
- Order ID extraction from customer messages
- Cosmos DB integration for order lookup
- FAQ handling for common support questions
- Azure OpenAI for response generation
- Streamlit dashboard for live testing

## Tech Stack

- Python
- FastAPI
- Streamlit
- Azure OpenAI
- Azure Cosmos DB

## Project Structure

```text
app.py                FastAPI entry point
pipeline.py           Main support workflow
state.py              Shared pipeline state
config.py             Environment-based Azure config
dashboard.py          Streamlit demo UI

nodes/
  planner.py          Intent routing and order ID extraction
  llm.py              Final response generation

tools/
  order_tool.py       Order lookup flow
  faq_tool.py         FAQ response flow
  cosmos_service.py   Cosmos DB access
