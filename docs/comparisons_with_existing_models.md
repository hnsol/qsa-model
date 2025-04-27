---
title: "Comparisons with Existing Models"
description: "Comparison between the QSA Model and related cognitive and agent frameworks."
target_audience: ["LLM", "Human"]
document_type: "Comparison"
tags: ["QSA", "LLM Reasoning", "Self-Ask", "ReAct", "Tree-of-Thought", "Auto-GPT"]
status: "draft"
created_at: "2025-04-27"
updated_at: "2025-04-27"
license: "MIT"
---

# Comparisons with Existing Models

## Self-Ask
- **Similarity**: Recursive self-questioning process.
- **Difference**: No explicit structure (S) phase; questions and answers intermingle.

## ReAct
- **Similarity**: Alternation between thought and action; stepwise reasoning.
- **Difference**: No distinct structure creation phase; focus on tool use and task execution.

## Tree-of-Thought
- **Similarity**: Structured exploration of reasoning paths (tree format).
- **Difference**: Tree structures multiple possible paths, not a single explicit structure per cycle.

## Autonomous Agents (Auto-GPT, BabyAGI)
- **Similarity**: Recursive planning, execution, and evaluation cycles.
- **Difference**: Focused on external task completion; QSA is about internal thought evolution.

## Human Cognitive Models
- **Similarity**: Echoes problem-solving cycles (e.g., Polya’s four steps).
- **Difference**: Human models are descriptive; QSA is prescriptive and operational for AI.

## Summary Table

| Model | Structure Explicit? | Recursive Thought? | Human-Initiated? | Designed for LLMs? |
|:------|:--------------------|:------------------|:----------------|:------------------|
| Self-Ask | No | Yes | Yes | Partially |
| ReAct | No | Yes | Yes | Yes |
| Tree-of-Thought | Yes (implicit) | Yes | Yes | Yes |
| Auto-GPT | Partially (planning) | Yes | No (after start) | Yes |
| QSA Model | **Yes (explicit S)** | **Yes (Q→S→A→Thought)** | **Yes (every cycle)** | **Yes** |
