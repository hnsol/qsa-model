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
language: ["en", "ja"]
---

# Comparisons with Existing Models / 既存モデルとの比較

---

## Self-Ask

- **Similarity / 類似点**: Recursive self-questioning process.  
  再帰的な自己問いかけのプロセス。
- **Difference / 相違点**: No explicit structure (S) phase; questions and answers intermingle.  
  明示的な構造（S）フェーズが存在せず、問いと答えが混在する。

---

## ReAct

- **Similarity / 類似点**: Alternation between thought and action; stepwise reasoning.  
  思考と行動の交互進行、段階的推論。
- **Difference / 相違点**: No distinct structure creation phase; focus on tool use and task execution.  
  構造生成フェーズが明示されず、ツール利用とタスク遂行に焦点が置かれている。

---

## Tree-of-Thought

- **Similarity / 類似点**: Structured exploration of reasoning paths (tree format).  
  推論経路の構造化探索（ツリー形式）。
- **Difference / 相違点**: Tree structures multiple possible paths, not a single explicit structure per cycle.  
  ツリーは複数経路を同時に構築するが、1サイクルごとの単一明示的構造ではない。

---

## Autonomous Agents (Auto-GPT, BabyAGI)

- **Similarity / 類似点**: Recursive planning, execution, and evaluation cycles.  
  再帰的な計画・実行・評価サイクル。
- **Difference / 相違点**: Focused on external task completion; QSA is about internal thought evolution.  
  外部タスク完了に焦点を当てるのに対し、QSAは内部思考進化に焦点を置く。

---

## Human Cognitive Models / 人間の認知モデル

- **Similarity / 類似点**: Echoes problem-solving cycles (e.g., Polya’s four steps).  
  問題解決サイクル（例：ポリアの四段階）に類似。
- **Difference / 相違点**: Human models are descriptive; QSA is prescriptive and operational for AI.  
  人間モデルは記述的だが、QSAは処方的かつAI実装指向である。

---

## Summary Table / まとめ表

| Model / モデル | Structure Explicit? / 構造明示? | Recursive Thought? / 再帰的思考? | Human-Initiated? / 人間主導? | Designed for LLMs? / LLM向け設計? |
|:------|:--------------------|:------------------|:----------------|:------------------|
| Self-Ask | No | Yes | Yes | Partially |
| ReAct | No | Yes | Yes | Yes |
| Tree-of-Thought | Yes (implicit) | Yes | Yes | Yes |
| Auto-GPT | Partially (planning) | Yes | No (after start) | Yes |
| QSA Model | **Yes (explicit S)** | **Yes (Q→S→A→Thought)** | **Yes (every cycle)** | **Yes** |

---

