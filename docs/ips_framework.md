---
title: "iPS Framework - Designing Thought Structures (S) in QSA / iPSフレームワーク - QSAにおける思考構造（S）の設計" # タイトル修正
description: "The iPS Framework (Intent, Plan, Scope) provides a lightweight guideline for humans (and potentially AI) to design the crucial Structure (S) phase within the QSA human-AI co-thinking protocol. / iPSフレームワーク（インテント、プラン、スコープ）は、人間（および潜在的にAI）が、人間-AI共同思考プロトコルであるQSAにおける重要な構造（S）フェーズを設計するための軽量ガイドラインです。" # 説明文修正
target_audience: ["LLM", "Human", "Developer", "Researcher"] # 対象読者追加
document_type: "Extension" # または "Component" も考えられる
tags: ["QSA", "iPS", "Structure Design", "Thought Process Design", "Human-AI Collaboration", "Cognitive Scaffolding", "Intent", "Plan", "Scope"] # タグ修正・追加
status: "published"
created_at: "2025-04-28"
updated_at: "2025-05-01" # 更新日 (仮)
license: "MIT"
language: ["en", "ja"]
---

# iPS Framework - Designing Thought Structures (S) in QSA / iPSフレームワーク - QSAにおける思考構造（S）の設計

---

## Purpose / 目的

The iPS Framework (Intent → Plan → Scope) is a lightweight, flexible guideline designed to assist **humans (primarily, but potentially also AI)** in consciously designing the **Structure (S) phase** of the QSA Model (Question → Structure → Answer → Thought). The 'S' phase is critical as it defines the reasoning framework for the subsequent 'A' (Answer) phase, often executed by an LLM within the **human-AI co-thinking protocol**.

（iPSフレームワーク（インテント→プラン→スコープ）は、**人間（主として、しかし潜在的にはAIも）**が QSAモデル（問い→構造→答え→思考）の**重要な構造（S）フェーズ**を意識的に設計するのを支援するために作られた、軽量で柔軟なガイドラインです。'S'フェーズは、**人間-AI共同思考プロトコル**内でしばしばLLMによって実行される後続の'A'（答え）フェーズの推論枠組みを定義するため、極めて重要です。）

iPS focuses on *how* to architect the thinking process for a given Question (Q) without mandating rigid formats, thereby facilitating clearer guidance for AI collaborators and more effective reasoning.
（iPSは、与えられた問い（Q）に対する思考プロセスを*どのように*構築するかに焦点を当て、厳密なフォーマットを強制することなく、AI協力者へのより明確なガイダンスと効果的な推論を促進します。）

---

## Core Content / コアコンテンツ

### Overview of iPS Flow within QSA's 'S' Phase / QSAの'S'フェーズ内でのiPSフロー概要

When tackling a Question (Q) in the QSA cycle, the iPS framework helps structure the 'S' phase by prompting consideration of:
（QSAサイクルで問い（Q）に取り組む際、iPSフレームワークは次の点を考慮するよう促すことで'S'フェーズの構造化を助けます：）

-   **Intent (インテント): What is the ultimate goal of answering Q?** Clearly define the desired outcome or purpose of this specific thinking cycle. *This sets the "why" for the Structure.*
    （**Qに答えることの最終ゴールは何か？** この特定の思考サイクルの望ましい成果や目的を明確に定義する。*これが構造の「なぜ」を設定する。*)
-   **Plan (プラン): How will we logically proceed to fulfill the Intent?** Draft a high-level strategy, sequence of steps, analytical framework, or reasoning path. *This outlines the "how" of the Structure.*
    （**インテントを達成するために、論理的にどう進むか？** 大局的な戦略、手順のシーケンス、分析フレームワーク、または推論パスの草案を作成する。*これが構造の「どのように」の概要を示す。*)
-   **Scope (スコープ): What are the boundaries and guiding principles?** Specify constraints, assumptions, perspectives to consider, information sources to use/avoid, level of detail required, etc. *This defines the "what" and "what not" of the Structure, shaping the reasoning space.*
    （**境界線と指針は何か？** 制約、仮定、考慮すべき視点、使用/回避すべき情報源、要求される詳細度などを指定する。*これが構造の「何を」「何でないか」を定義し、推論空間を形成する。*)

Completing an iPS thought process yields the **Structure (S)**, which then serves as the explicit foundation for generating the **Answer (A)**, often by an LLM.
（iPSの思考プロセスを完了すると**構造（S）**が得られ、それが次に、しばしばLLMによって**答え（A）**を生成するための明示的な基盤として機能します。）

---

### Relation to Prompting Techniques & Human-AI Collaboration / プロンプト技術および人間-AI協働との関係

iPS operates at a **meta-level** compared to specific LLM prompting techniques (CoT, ReAct, etc.).
（iPSは、特定のLLMプロンプト技術（CoT, ReActなど）と比較して**メタレベル**で機能します。）

-   **Structuring the Human Input:** iPS primarily structures the **human's contribution to the 'S' phase**. It helps the human clarify their thinking *before* instructing the AI (or collaborating with the AI on 'S'). This leads to better-defined 'S' structures, which in turn enable the LLM to generate more relevant and coherent 'A' answers.
    （**人間の入力の構造化：** iPSは主として**'S'フェーズへの人間の貢献**を構造化します。AIに指示を出す前（またはAIと'S'について協働する前）に、人間が自身の思考を明確化するのを助けます。これにより、より良く定義された'S'構造が生まれ、結果としてLLMがより関連性の高い一貫した'A'の答えを生成できるようになります。）
-   **Complementary, Not Exclusive:** An iPS-defined 'Plan' within 'S' might *specify* using a CoT approach for a particular sub-task, or the 'Scope' might define which tools are permissible (relevant to ReAct). iPS provides the overarching architecture; prompting techniques are tools used within that architecture.
    （**排他的ではなく補完的：** 'S'内のiPSで定義された'Plan'は、特定のサブタスクにCoTアプローチを使用することを*指定*するかもしれませんし、'Scope'はどのツールが許可されるか（ReActに関連）を定義するかもしれません。iPSは全体的なアーキテクチャを提供し、プロンプト技術はそのアーキテクチャ内で使用されるツールです。）
-   **Facilitating Co-Creation of 'S':** While primarily human-guided, the iPS framework can also structure a dialogue where a human defines the Intent, and then collaborates with an LLM to brainstorm or refine the Plan and Scope for the 'S' phase.
    （**'S'の共創促進：** 主として人間がガイドしますが、iPSフレームワークは、人間がインテントを定義し、その後LLMと協働して'S'フェーズのためのプランとスコープをブレインストーミングまたは洗練する対話を構造化することもできます。）

In essence, iPS acts as **cognitive scaffolding** for designing the crucial 'S' structure within the QSA protocol, thereby enhancing the effectiveness of the human-AI collaborative reasoning process.
（本質的に、iPSはQSAプロトコル内の重要な'S'構造を設計するための**認知的足場（cognitive scaffolding）**として機能し、それによって人間-AI協調推論プロセスの有効性を高めます。）

---

## Key Points / 重要ポイント

-   **Enhances QSA's 'S' Phase:** Provides a structured way to design the critical Structure component.
    （**QSAの'S'フェーズを強化：**重要な構造コンポーネントを設計するための構造化された方法を提供。）
-   **Focus on Thought Design:** Prioritizes *how* to think (Intent, Plan, Scope) over specific output formats.
    （**思考設計への焦点：**特定の出力形式よりも、*どのように*考えるか（インテント、プラン、スコープ）を優先。）
-   **Improves Human-AI Communication:** Creates clearer instructions/context for LLM collaborators by structuring the human thought process first.
    （**人間-AIコミュニケーションを改善：**人間の思考プロセスを最初に構造化することで、LLM協力者へのより明確な指示/コンテキストを作成。）
-   **Flexible & Lightweight:** Minimal core elements (Intent, Plan), adaptable guideline.
    （**柔軟＆軽量：**最小限のコア要素（インテント、プラン）、適応可能なガイドライン。）
-   **Format Agnostic:** Does not prescribe YAML, JSON, etc., for its output (the 'S' structure itself might use those).
    （**フォーマット非依存：**そのアウトプット（'S'構造自体はそれらを使うかもしれないが）にYAML、JSONなどを規定しない。）

---

## Related Topics (Optional) / 関連トピック（任意）

-   [QSA Model Overview](../concept_overview.md) # 相対パス修正
-   [QSA Comparisons with Existing Models](../comparisons_with_existing_models.md) # 相対パス修正

---

## Future Work (Optional) / 将来展望（任意）

-   Develop interactive tools that guide users through the iPS process to generate 'S' structures for QSA.
    （ユーザーをiPSプロセスを通してガイドし、QSAのための'S'構造を生成するインタラクティブツールの開発。）
-   Investigate LLM capabilities in autonomously generating or critiquing iPS components (Intent, Plan, Scope) based on an initial Question (Q).
    （初期の問い（Q）に基づき、iPSコンポーネント（インテント、プラン、スコープ）を自律的に生成または批評するLLMの能力を調査。）
-   Formalize iPS patterns for common reasoning tasks (e.g., problem diagnosis, strategic planning, creative brainstorming).
    （一般的な推論タスク（問題診断、戦略計画、創造的ブレインストーミングなど）のためのiPSパターンの定式化。）

---
