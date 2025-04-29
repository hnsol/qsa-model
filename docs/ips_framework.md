---
title: "iPS Framework - Intent, Plan, Scope for Thought Process Design / iPSフレームワーク - 思考プロセス設計のためのインテント、プラン、スコープ"
description: "The iPS Framework provides a lightweight and flexible guideline for designing structured thinking processes within the Structure (S) phase of the QSA Model. / iPSフレームワークは、QSAモデルの構造（S）フェーズにおいて、思考プロセスを構造化するための軽量かつ柔軟なガイドラインです。"
target_audience: ["LLM", "Human"]
document_type: "Extension"
tags: ["QSA", "LLM Reasoning", "Extension", "iPS", "Thought Process Design"]
status: "published"
created_at: "2025-04-28"
updated_at: "2025-04-29"
license: "MIT"
language: ["en", "ja"]
---

# iPS Framework - Intent, Plan, Scope for Thought Process Design / iPSフレームワーク - 思考プロセス設計のためのインテント、プラン、スコープ

---

## Purpose / 目的

The iPS Framework (Intent → Plan → Scope) is a lightweight guideline for designing the thought process, complementing the Structure (S) phase of the QSA Model (Question → Structure → Answer → Thought).  
（iPSフレームワーク（インテント→プラン→スコープ）は、QSAモデル（問い→構造→答え→思考）の「構造（S）」フェーズを補完する、思考プロセス設計のための軽量なガイドラインです。）

It focuses on how to organize thinking flexibly without prescribing specific data formats (like YAML/JSON) or rigid prompting templates.  
（特定のデータ形式（YAML/JSONなど）や厳密なプロンプトテンプレートを規定せず、思考をどのように柔軟に構造化するかに焦点を当てます。）

---

## Core Content / コアコンテンツ

### Overview of iPS Flow / iPSフロー概要

The iPS Framework structures thinking into three stages:

（iPSフレームワークは、思考を次の3段階に構造化します：）

- **Intent (インテント)**: Clearly define the ultimate goal or aim of the thinking activity.  
  （思考活動における最終ゴールや目的を明確にする。）

- **Plan (プラン)**: Draft a logical path or strategy for reaching the Intent.  
  （インテント達成に向けた論理的な道筋や設計を描く。）

- **Scope (スコープ)**: Specify boundaries, constraints, and guiding conditions to shape the thinking space without limiting creativity.  
  （創造性を制限することなく、思考空間を形成するための境界条件、制約条件、指針を設定する。）

---

### Relation to Prompting Techniques / プロンプト技術との関係

iPS operates at a higher level of abstraction compared to common prompting techniques such as Chain of Thought (CoT), Self-Ask, or ReAct.  
（iPSは、Chain of Thought（CoT）、Self-Ask、ReActといった一般的なプロンプト技術よりも高い抽象レベルで機能します。）

- **Focus Level / 焦点レベル**:  
  Prompting techniques typically instruct *how an LLM should execute a task* (e.g., "think step-by-step"), whereas iPS focuses on *designing the overall flow of thought* prior to prompt execution.  
  （プロンプト技術は通常、LLMがタスクを*どのように実行すべきか*を指示しますが、iPSはそれ以前に*思考の全体フロー*を設計することに焦点を当てます。）

- **Flexibility / 柔軟性**:  
  Prompting formats often impose specific steps or structures. iPS offers flexible thinking architecture, allowing incorporation of methods like CoT or Self-Ask within a broader, adaptive framework.  
  （プロンプト形式は特定の手順や構造を要求することが多いですが、iPSはより広範で適応的なフレームワークの中で、CoTやSelf-Askのような方法を柔軟に取り入れることを可能にします。）

- **Goal / 目標**:  
  iPS structures the *human side* of the thought process, clarifying purpose and logical flow before specific prompt construction.  
  （iPSは思考プロセスにおける*人間側*を構造化し、具体的なプロンプト構築に先立って目的と論理的流れを明確にします。）

Thus, iPS complements prompting techniques by operating at a meta-level of thought design.  
（したがって、iPSは思考設計のメタレベルで機能し、プロンプト技術を補完します。）

---

## Key Points / 重要ポイント

- **Flexibility / 柔軟性**: Supports both pure exploration and practical application.  
  （純粋な探究にも実務的応用にも対応可能。）

- **Process-Oriented / プロセス志向**: Prioritizes structuring the flow of thought itself.  
  （思考の流れ自体を構造化することを重視。）

- **Clarity / 明確性**: Explicitly defines goals and boundary conditions.  
  （ゴールと境界条件を明確に定義する。）

- **Minimalism / ミニマリズム**: Only Intent and Plan are mandatory; Scope is highly recommended but flexible.  
  （インテントとプランは必須、スコープは推奨だが柔軟。）

- **Guideline, Not Template / ガイドラインでありテンプレートではない**: Offers freedom in specific implementations.  
  （具体的な実装に自由度を持たせる。）

---

## Related Topics (Optional) / 関連トピック（任意）

- [QSA Model Overview](./concept_overview.md)  
（QSAモデル概要へのリンク）

- [Deep Research on QSA Originality](./deep_research_on_originality.md)  
（QSAの独自性に関するディープリサーチへのリンク）

---

## Future Work (Optional) / 将来展望（任意）

- Develop IPS-based structured brainstorming templates.  
  （IPSに基づく構造化ブレインストーミングテンプレートを開発する。）

- Explore Scope-driven reasoning in agent architectures.  
  （スコープ主導型推論を用いたエージェント設計の探究。）

---
