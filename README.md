# Playwright-MCP-CoPilot-Project
This repository demonstrates a prompt-driven test automation framework built using Playwright (Python), PlaywrightMCP (Model Context Protocol), and GitHub Copilot.

In this approach, test intent is written as natural language prompts. GitHub Copilot uses Playwright MCP to understand the project context, and test structure, generates Playwright test scripts from the prompt, and executes them. Test results are displayed directly in PyCharm, as per the instructions set in Prompt

Prompt (natural language)
        ↓
Playwright MCP
        ↓
GitHub Copilot (PyCharm)
        ↓
Test script generation (Playwright (Python))
        ↓
Test execution
        ↓
Test execution results generated

What actually happens
------------------------

1. Test intent is written as a prompt file
2. Playwright MCP exposes Playwright Python capabilities and context
3. GitHub Copilot:
  - Reads the prompt
  - Understands the Playwright Python APIs via MCP
  - Generates Playwright test scripts
4. Generated tests are executed using Playwright
5. Execution results (pass/fail, logs, screenshots) are shown in PyCharm

No custom MCP server is used — the project relies on Playwright MCP.

