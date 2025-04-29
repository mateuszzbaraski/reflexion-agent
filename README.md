# Reflection Agent with Real-Time Search and Critique Loop

## Overview

This project implements a **Reflection Agent** that:

- Generates high-quality articles on a given topic.
- Fetches **real-time information** using an external search tool.
- Iteratively **critiques and improves** its outputs based on retrieved data.
- Provides proper **citations** for sourced information.

The agent uses an advanced feedback loop to enhance response quality through multiple revisions.

## Architecture

1. **Responder Node**

   - Generates an initial article, critique, and proposed search terms.

2. **Execute Tools Node**

   - Runs real-time search queries (via [Tavily](https://www.tavily.com/)) to gather external data.

3. **Reviser Node**

   - Incorporates critique and new search results.
   - Revises the article, adds citations, and suggests new search terms.

4. **Iteration Loop**
   - Continues refining until a stopping condition is reached.

## Technologies

- **OpenAI GPT Model** (e.g., GPT-4) for text generation and critique.
- **Tavily API** for real-time web search.
- **LangGraph** for flow orchestration.
- **LangSmith** for tracing and debugging.
- **Function Calling** for structured tool execution.

## Setup

The code is available on the GitHub repository under the `reflection-agent` branch.  
Each commit corresponds to a tutorial step for easy reference.
