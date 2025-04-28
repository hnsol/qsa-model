---
title: iPS Framework - Intent, Process, (Strategy) for Thought Process Design / iPSフレームワーク - 思考プロセス設計のためのインテント、プロセス、（ストラテジー）
created_at: 2025-04-28
updated_at: 2025-04-28
description: "The iPS Framework (Intent, Process, (Strategy)) is a lightweight guideline for designing the thought process within the Structure (S) phase of the QSA Model, enabling flexible adaptation and evolution. / iPSフレームワーク（インテント、プロセス、（ストラテジー））は、QSAモデルの構造（S）フェーズ内における思考プロセス設計のための軽量なガイドラインであり、柔軟な適応と進化を可能にします。"
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

The iPS Framework (Intent → Process → (Strategy)) is a lightweight **guideline for designing the thought process**, complementing the Structure (S) phase of the QSA Model (Question → Structure → Answer → Thought). **It focuses on *how* to structure thinking, rather than prescribing specific data formats (like YAML/JSON) or prompt templates.**

iPSフレームワーク（インテント→プロセス→（ストラテジー））は、QSAモデル（問い→構造→答え→思考）の「構造（S）」フェーズを補完する、**思考プロセス設計のための軽量なガイドライン**です。**これは、特定のデータ形式（YAML/JSONなど）やプロンプトテンプレートを規定するのではなく、思考を *どのように* 構造化するかに焦点を当てます。**

Inspired by the concept of iPS cells, it acts as a "thought stem cell," allowing structured thinking to flexibly adapt and evolve toward either pure inquiry or practical application.

iPS細胞の概念に着想を得て、純粋な探究型思考にも、実践的応用型思考にも自在に分化できる「思考の幹細胞」として機能します。

---

## Core Content / コアコンテンツ

### Overview / 概要

iPS Framework defines a three-stage flow for designing the thinking process:

iPSフレームワークは、思考プロセスを設計するための3段階のフローを定義します：

- **Intent (インテント)**: Clearly articulate the **aim or purpose** of the thinking activity for the current cycle. / 現在のサイクルにおける思考活動の**狙いや目的**を明確にする。
- **Process (プロセス)**: Design the **logical structure or pathway** (e.g., steps, perspectives, analysis points) to achieve the intent. / インテントを達成するための**論理的な構造や経路**（例：ステップ、観点、分析ポイント）を設計する。
- **(Strategy) (ストラテジー)** *(Optional)*: Optionally design a **future deployment, action plan, or direction for application** based on the anticipated outcome. / 期待される成果に基づき、**将来の展開、アクションプラン、または応用方向**を任意で設計する。

Strategy is optional, preserving the freedom for pure thought exploration when needed.

ストラテジーは任意要素であり、純粋な思考探究を重視する場合には省略可能です。

---

## Relation to Prompting Techniques / プロンプト技術との関係

**iPS is distinct from common prompting techniques like Chain of Thought (CoT), Self-Ask, or ReAct.**

**iPSは、Chain of Thought (CoT), Self-Ask, ReActといった一般的なプロンプト技術とは異なります。**

- **Focus Level / 焦点レベル**: Prompting techniques typically provide **specific instructions or templates** for *how LLMs should execute a task* (e.g., "think step-by-step"). iPS operates at a higher level, focusing on **designing the *overall thought process* (Intent, Process, Strategy)** *before* crafting specific prompts or structuring data. / プロンプト技術は通常、LLMがタスクを*どのように実行すべきか*についての**具体的な指示やテンプレート**（例：「ステップバイステップで考えて」）を提供します。iPSはより上位のレベルで機能し、具体的なプロンプトを作成したりデータを構造化したりする*前*に、**思考プロセス全体（インテント、プロセス、ストラテジー）を設計する**ことに焦点を当てます。

- **Flexibility / 柔軟性**: While prompting techniques often follow a defined format, iPS is a **flexible guideline**. The Process designed using iPS can be implemented using various methods, potentially incorporating elements of CoT or Self-Ask within specific steps if appropriate for the task. / プロンプト技術はしばしば定義された形式に従いますが、iPSは**柔軟なガイドライン**です。iPSを用いて設計されたプロセスは、様々な方法で実装可能であり、タスクに応じて特定のステップ内でCoTやSelf-Askの要素を部分的に組み込むことも可能です。

- **Goal / 目標**: iPS primarily aims to **structure the *human's* thinking about the thinking process itself**, ensuring clarity of purpose and logical flow, which then informs how the Structure (S) phase is implemented for the LLM. / iPSの主な目的は、**思考プロセス自体に関する*人間*の思考を構造化**し、目的の明確さと論理的な流れを確保することです。これが、LLMのための構造（S）フェーズをどのように実装するかの指針となります。

---

## Example of Connecting iPS to S Implementation / iPSからS実装への接続例

Let's consider the "Open vs. Closed Questions" example:

「オープン質問 vs クローズ質問」の例を考えます：

1. **iPS Design / iPSによる設計:**
    * `Intent`: Understand the nuances of using open and closed questions in a 1-on-1 meeting to boost motivation. / 1on1ミーティングでモチベーションを高めるための、オープン質問とクローズ質問の使い方のニュアンスを理解する。
    * `Process`: 1. Define terms → 2. Compare benefits/drawbacks in 1-on-1 context → 3. Identify specific motivational scenarios → 4. Generate example question sequences for each scenario → 5. Summarize key principles. / 1. 用語定義 → 2. 1on1文脈でのメリット/デメリット比較 → 3. 具体的な動機付けシナリオ特定 → 4. 各シナリオの質問シーケンス例生成 → 5. 主要原則の要約。
    * `(Strategy)`: Create a checklist for managers based on these principles. / これらの原則に基づきマネージャー向けのチェックリストを作成する。

2. **Potential S Implementations / Sの実装例:**
    * **Option A (Structured Prompt):** Create a detailed Markdown prompt for the LLM that outlines the 5 steps defined in the `Process`, possibly instructing it to "think step-by-step" (using CoT idea) for each step. / `Process`で定義された5つのステップを概説する詳細なMarkdownプロンプトを作成し、各ステップで「ステップバイステップで考える」ように指示する（CoTの考え方を使用）。
    * **Option B (Iterative Prompts):** Break down the `Process` into 5 separate prompts, feeding the output of one step as context for the next. / `Process`を5つの個別のプロンプトに分割し、あるステップの出力を次のステップのコンテキストとして与える。
    * **Option C (Data Schema):** Define a JSON structure representing the desired output (e.g., fields for scenario, open question example, closed question example, rationale) and instruct the LLM to fill it based on its knowledge. / 望ましい出力を表現するJSON構造（例：シナリオ、オープン質問例、クローズ質問例、根拠などのフィールド）を定義し、LLMにその知識に基づいて入力するよう指示する。

**iPS guides the *design* of the thinking flow; the specific implementation of 'S' (the input to the LLM) can vary.**

**iPSは思考フローの*設計*を導き、具体的な'S'（LLMへの入力）の実装方法は様々です。**

---

## Application in QSA / QSAモデルとの関係

- The iPS Framework operates **within the Structure (S)** phase of the QSA model **as a guideline for designing the thinking process**. / iPSフレームワークは、QSAモデルにおける「構造（S）」フェーズ内で、**思考プロセスを設計するためのガイドラインとして**運用されます。

- It allows the Structure phase to flexibly: / Sフェーズにおいて、次のような柔軟運用を可能にします：
  - Focus purely on logical organization (Intent + Process only) / 純粋に論理構成の設計に集中（インテント＋プロセスのみ）
  - Or extend toward action and future evolution (Intent + Process + Strategy) / 必要に応じて未来展開まで設計（インテント＋プロセス＋ストラテジー）

By integrating iPS, QSA can elegantly balance **pure inquiry** and **real-world applicability** without distorting its core cyclic nature. **iPS helps ensure the 'S' phase is purposeful and well-structured before specific prompts or data formats are finalized.**

iPSを統合することで、QSAの本質的な循環性を損なうことなく、純粋探究と思考の現実適用を優雅に両立できます。**iPSは、具体的なプロンプトやデータ形式が最終決定される前に、「S」フェーズが意図的でよく構造化されていることを保証するのに役立ちます。**

---

## Key Points / 重要ポイント

- **Flexibility / 柔軟性**: Adapts to both pure theoretical exploration and action-oriented thinking. / 純粋な理論的探求と思考の現実適用の両方に適応。
- **Process-Oriented / プロセス指向**: Focuses on **designing the flow of thought**, not just the output format. / 思考のフロー設計に焦点を当て、単なる出力形式だけではない。
- **Minimalism / ミニマリズム**: Only Intent and Process are required; Strategy is optional. / インテントとプロセスのみ必須、ストラテジーは任意。
- **Future-readiness / 未来接続性**: Enables next-step generation and real-world application when needed. / 必要に応じて次のステップ生成や実世界応用を可能にする。
- **Guideline, Not Rigid Format / ガイドラインであり、厳密な形式ではない**: Provides a mental model to structure thinking, complementing various implementation methods (prompts, structured data). / 思考を構造化するためのメンタルモデルを提供し、様々な実装方法（プロンプト、構造化データ）を補完する。

---

## Related Topics (Optional) / 関連トピック（任意）

- [QSA Model Overview](./concept_overview.md)
- [Deep Research on Originality of QSA](./deep_research_on_originality.md)
- **(Optional) Link to a document explaining common prompting techniques like CoT, Self-Ask.** / （任意）CoTやSelf-Askのような一般的なプロンプト技術を説明するドキュメントへのリンク。

---

## Future Work (Optional) / 将来展望（任意）

- Develop "iPS-Enhanced Templates" for structured brainstorming sessions **(clarifying how iPS informs template structure)**. / 構造的ブレインストーミング用の「iPS拡張テンプレート」を開発する（iPSがテンプレート構造にどう影響するかを明確にする）。
- Explore interaction models between iPS and various types of LLM agents. / iPSと多様なLLMエージェントとのインタラクションモデルを探究する。
- Refine the Strategy phase into optional micro-frameworks for different domains (e.g., scientific research, product design). / ストラテジーフェーズをドメイン別（例：科学研究、製品設計）に応じたオプション型マイクロフレームワークへと精緻化する。
