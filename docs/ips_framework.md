---
title: iPS Framework - Intent, Plan, Scope for Thought Process Design / iPSフレームワーク - 思考プロセス設計のためのインテント、プラン、スコープ
created_at: 2025-04-28
updated_at: 2025-04-29
description: "The iPS Framework (Intent, Plan, Scope) is a lightweight guideline for designing the thought process within the Structure (S) phase of the QSA Model, enabling flexible adaptation and evolution. / iPSフレームワーク（インテント、プラン、スコープ）は、QSAモデルの構造（S）フェーズ内における思考プロセス設計のための軽量なガイドラインであり、柔軟な適応と進化を可能にします。"
target_audience:
  - LLM
  - Human
document_type: Extension
tags:
  - QSA
  - LLM Reasoning
  - Extension
  - iPS
  - Thought Process Design
status: completed
license: MIT
language:
  - en
  - ja
---

## Purpose / 目的

The iPS Framework (Intent → Plan → Scope) is a lightweight **guideline for designing the thought process**, complementing the Structure (S) phase of the QSA Model (Question → Structure → Answer → Thought).  
（iPSフレームワーク（インテント→プラン→スコープ）は、QSAモデル（問い→構造→答え→思考）の「構造（S）」フェーズを補完する、思考プロセス設計のための軽量なガイドラインです。）

It focuses on *how to organize thinking* flexibly, without prescribing specific data formats (like YAML/JSON) or fixed prompting templates.  
（特定のデータ形式（YAML/JSONなど）や固定プロンプトテンプレートを規定するのではなく、思考をどのように構造化するかに柔軟に焦点を当てます。）

---

## Core Content / コアコンテンツ

### Overview / 概要

The iPS Framework defines a three-stage flow for structuring thinking:  
（iPSフレームワークは、思考を構造化するための3段階のフローを定義します。）

- **Intent (インテント)**: Clearly define the **ultimate goal or aim** of the thinking activity.  
  （思考活動における最終ゴールや目的を明確にする。）

- **Plan (プラン)**: Draft a **logical path or strategy** for reaching the Intent.  
  （インテント達成のための論理的な道筋や設計を描く。）

- **Scope (スコープ)**: Specify **boundaries, constraints, and guiding conditions** to shape the thinking space without limiting creativity.  
  （創造性を制限することなく、思考空間を形作るための境界条件、制約条件、指針を明示する。）

Scope enables structured freedom, ensuring that LLMs or humans operate flexibly within meaningful parameters.  
（スコープは、意味のある範囲内でLLMや人間が柔軟に思考できるように設計されます。）

---

## Relation to Prompting Techniques / プロンプト技術との関係

**iPS is distinct from typical prompting techniques such as Chain of Thought (CoT), Self-Ask, or ReAct.**  
（iPSは、Chain of Thought（CoT）、Self-Ask、ReActなどの一般的なプロンプト技術とは異なります。）

- **Focus Level / 焦点レベル**: Prompting techniques guide *how to execute* a given task, while iPS operates *before* that, designing the overall *thought architecture*.  
  （プロンプト技術はタスク遂行方法を指示しますが、iPSはその前段階で思考の構造全体を設計します。）

- **Flexibility / 柔軟性**: iPS is not bound by specific formats. The Plan and Scope can dynamically accommodate different reasoning styles and prompting methods.  
  （iPSは特定の形式に縛られず、プランとスコープを通じて異なる推論スタイルやプロンプト方法に柔軟に適応できます。）

- **Goal / 目標**: iPS aims to **structure the human side of the thought process**, enabling clearer communication with LLMs or among collaborators.  
  （iPSは思考プロセスにおける人間側の構造化を目指し、LLMや共同作業者とのより明確な対話を可能にします。）

---

## Example of Connecting iPS to S Implementation / iPSからS実装への接続例

For example:  
（例：）

1. **iPS Design / iPSによる設計:**
    * `Intent`: Explore optimal question design strategies in 1-on-1 meetings.  
      （1on1ミーティングにおける最適な質問設計戦略を探究する。）
    * `Plan`: Define open vs. closed questions → Compare psychological impacts → Generate examples and heuristics.  
      （オープン質問とクローズ質問を定義 → 心理的影響を比較 → 例とヒューリスティクスを生成。）
    * `Scope`: Focus only on professional contexts; exclude casual conversations.  
      （プロフェッショナルな文脈のみに焦点を当て、カジュアルな会話は除外する。）

2. **Possible S Implementations / Sの実装例:**
    - Structured prompt following the Plan steps.  
      （プランのステップに従った構造的プロンプトを作成する。）
    - JSON output schema shaped by the Scope conditions.  
      （スコープ条件に基づいたJSON出力スキーマを設計する。）

---

## Application in QSA / QSAモデルとの関係

The iPS Framework operates **within the Structure (S) phase** of QSA, providing a mental model for *how to design* the thinking structure before implementation.  
（iPSフレームワークは、QSAモデルの「構造（S）」フェーズ内で、実装に先立つ思考構造の設計を支援するメンタルモデルとして機能します。）

It preserves the recursive, cyclic nature of QSA while adapting flexibly to either pure inquiry or practical application.  
（QSAの本質的な循環性を維持しながら、純粋探究にも実務応用にも柔軟に適応できる設計を可能にします。）

---

## Key Points / 重要ポイント

- **Flexibility / 柔軟性**: Supports both pure exploration and real-world application.  
  （純粋探究にも実務応用にも適応できる。）

- **Process-Oriented / プロセス指向**: Emphasizes designing the thinking flow itself, not just outputs.  
  （出力だけでなく、思考フロー自体の設計を重視する。）

- **Minimalism / ミニマリズム**: Only Intent and Plan are mandatory; Scope is highly recommended but flexible.  
  （インテントとプランは必須、スコープは推奨されるが柔軟。）

- **Clarity / 明確性**: Makes the thinking purpose and boundary conditions explicit.  
  （思考目的と境界条件を明確にする。）

- **Guideline, Not Template / ガイドラインでありテンプレートではない**: Offers a flexible mental model, not rigid step-by-step instructions.  
  （固定手順ではなく柔軟なメンタルモデルを提供する。）

---

## Future Work (Optional) / 将来展望（任意）

- Develop IPS-driven templates for structured brainstorming.  
  （IPS設計に基づく構造化ブレインストーミングテンプレートの開発。）

- Explore deeper integrations of Scope-driven reasoning in LLM agent design.  
  （スコープ設計に基づくLLMエージェント設計との統合探究。）

---
