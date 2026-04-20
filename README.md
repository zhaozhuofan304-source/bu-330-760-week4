# Week 4 Starter: Math Agent

A ReAct agent that solves questions using tool calls.

## Setup

1. Install [uv](https://docs.astral.sh/uv/getting-started/installation/) if you don't have it.

2. Copy `.env.example` to `.env` and add your API key:
   ```bash
   cp .env.example .env
   ```
   Then edit `.env` and replace `your-key-here` with your key from [Google AI Studio](https://aistudio.google.com/apikey).

   To use a different provider, change the `MODEL` variable in `agent.py` and set the matching key in `.env`.

3. Make sure `.env` is in your `.gitignore` so you don't commit your key.

## Run

```bash
uv run agent.py
```

uv will install dependencies automatically on first run.

The agent will work through each question in `math_questions.md` and print the ReAct trace (Reason / Act / Result) for each one.

## Files

- `agent.py` - the ReAct agent (this is the file you'll modify)
- `calculator.py` - calculator tool
- `products.json` - product catalog with prices
- `math_questions.md` - the questions the agent solves
- `.env.example` - template for your API key
  
# Math Agent with Tool Use
This project implements a ReAct-style math agent with two tools:
- `calculator_tool` for arithmetic
- `product_lookup` for catalog price lookup from `products.json`

The missing `product_lookup` tool was implemented in `agent.py`.  
The agent can use the calculator for math questions and the catalog lookup tool for product price questions.

## Demo Video
PASTE_YOUR_VIDEO_LINK_HERE
