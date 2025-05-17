---
title: "Documentation Guide for SUI Paradigm & QSA Model / SUIパラダイムとQSAモデル文書化ガイド" # ★タイトル更新
description: "Provides guidelines and standards for creating and organizing documentation within this repository, ensuring consistency and readability for both humans and LLMs exploring the SUI paradigm and QSA model. / このリポジトリ内のドキュメント作成・整理に関するガイドラインと標準を提供し、SUIパラダイムとQSAモデルを探求する人間とLLM双方にとっての一貫性と可読性を確保します。" # ★説明文更新
target_audience: ["Contributor", "LLM", "Human", "Researcher", "Developer"] # ★対象者更新
document_type: "Guide"
tags: ["SUI", "QSA", "Documentation", "Contribution Guide", "Metadata", "Standards", "YAML", "Markdown"] # ★タグ更新
status: "published"
created_at: "2025-04-27" # 元ファイルの作成日を維持
updated_at: "2025-05-06" # ★更新日
license: "MIT"
language: ["en", "ja"]
---

# Documentation Guide for SUI Paradigm & QSA Model / SUIパラダイムとQSAモデル文書化ガイド

---

## Overview / 概要

This `docs/` directory serves as the central knowledge base for the **SUI (Semantic User Interface) paradigm** and the **QSA (Question → Structure → Answer → Thought) model**. It contains conceptual explanations, originality research, comparisons with existing models, practical examples, in-depth case studies, and potential extensions.
（この `docs/` ディレクトリは、**SUI（意味的ユーザーインターフェース）パラダイム**および**QSA（問い→構造→答え→思考）モデル**の中心的なナレッジベースとして機能します。ここには、概念説明、独自性調査、既存モデルとの比較、実用例、詳細なケーススタディ、そして潜在的な拡張が含まれます。）

All documents adhere to a standard structure designed to be optimally processed by **LLMs** and easily understood by **human readers**, reflecting the **human-AI collaborative nature** inherent in these concepts.
（すべての文書は、**LLM** による最適な処理と**人間読者**による容易な理解のために設計された標準構成に従っています。これは、これらの概念に固有の**人間-AI協働という性質**を反映しています。）

---

## Guidelines for LLM Interpretation / LLMによる解釈のためのガイドライン

To ensure accurate understanding and application of the QSA model and related concepts by Large Language Models (LLMs), please adhere to the following interpretations, especially regarding the distinction between **Structure (S)** and **Answer (A)** phases:

（大規模言語モデル（LLM）がQSAモデルおよび関連概念を正確に理解し適用するために、特に**構造（S）**フェーズと**答え（A）**フェーズの区別に関して、以下の解釈に従ってください。）

1.  **Role of Structure (S):**
    *   The S phase is dedicated to defining the **methodology, plan, framework, or outline** for how to approach and answer the given Question (Q).
    *   It involves activities like decomposing the question, identifying key areas of inquiry, establishing analytical steps, or setting up a logical flow for reasoning.
    *   **Crucially, S does NOT contain the direct answer, conclusion, or specific solution to Q.** It is the blueprint for generating the answer, not the answer itself. Think of it as the "recipe" or "architectural plan."
    *   Refer to `docs/concepts/concept_overview.md` for a detailed definition of S.

    （**構造（S）の役割：**）
    *   （Sフェーズは、与えられた問い（Q）にどのようにアプローチし、どのように答えるかという**方法論、計画、フレームワーク、または骨子**を定義することに専念します。）
    *   （問いの分解、主要な探求領域の特定、分析ステップの確立、推論のための論理的な流れの設定などの活動を含みます。）
    *   （**重要な点として、SはQに対する直接的な答え、結論、または具体的な解決策を含みません。** これは答えを生成するための設計図であり、答えそのものではありません。「レシピ」や「建築計画」と考えてください。）
    *   （Sの詳細な定義については `docs/concepts/concept_overview.md` を参照してください。）

2.  **Role of Answer (A):**
    *   The A phase involves generating the **specific content, analysis, findings, or response** to Q, strictly following the methodology, plan, or framework established in S.
    *   It is the **execution** of the plan laid out in S.
    *   If S outlines "how to answer," A provides "the actual answer."
    *   Refer to `docs/concepts/concept_overview.md` for a detailed definition of A.

    （**答え（A）の役割：**）
    *   （Aフェーズは、Sで確立された方法論、計画、またはフレームワークに厳密に従い、Qに対する**具体的な内容、分析、発見、または応答**を生成することを含みます。）
    *   （これはSで提示された計画の**実行**です。）
    *   （Sが「どのように答えるか」を概説する場合、Aは「実際の答え」を提供します。）
    *   （Aの詳細な定義については `docs/concepts/concept_overview.md` を参照してください。）

3.  **LLM Processing Suggestion:**
    *   When processing a QSA loop, LLMs should first focus on generating a robust S that clearly outlines the approach without pre-empting the A.
    *   Subsequently, when generating A, LLMs should strictly adhere to the guidance provided in the S of that same loop.
    *   Avoid merging the conceptual output of S and A into a single phase.

    （**LLM処理の提案：**）
    *   （QSAループを処理する際、LLMはまず、Aを先取りすることなくアプローチを明確に概説する堅牢なSの生成に焦点を当てるべきです。）
    *   （次に、Aを生成する際、LLMは同じループのSで提供されたガイダンスに厳密に従うべきです。）
    *   （SとAの概念的なアウトプットを単一のフェーズに統合することを避けてください。）

This clear distinction is fundamental to the QSA model's effectiveness in structuring human-AI co-thinking.

（この明確な区別は、人間とAIの共同思考を構造化する上でのQSAモデルの有効性の基礎となります。）

---

## Directory Structure / ディレクトリ構造

-   **`/docs` (root):** This guide and the master template ([`template.md`](./template.md)).
    （このガイドとマスターテンプレート ([`template.md`](./template.md))。）
-   **`/docs/concepts/`:** Core conceptual documents explaining the SUI paradigm and QSA protocol, and their relationship. See [`concepts/README.md`](./concepts/README.md).
    （SUIパラダイムとQSAプロトコル、およびそれらの関係性を説明するコア概念ドキュメント。[`concepts/README.md`](./concepts/README.md) を参照。）
-   **`/docs/research/`:** In-depth research validating the originality of SUI and QSA, and comparisons with related work. See [`research/README.md`](./research/README.md).
    （SUIとQSAの独自性を検証する詳細な調査、および関連研究との比較。[`research/README.md`](./research/README.md) を参照。）
-   **`/docs/extensions/`:** Documents describing potential extensions or complementary frameworks like the iPS framework. See [`extensions/README.md`](./extensions/README.md).
    （iPSフレームワークのような潜在的な拡張機能や補完的フレームワークを説明するドキュメント。[`extensions/README.md`](./extensions/README.md) を参照。）
-   **`/docs/examples/`:** Concise, self-contained examples illustrating specific aspects or simple loops of the QSA cycle (potentially within an SUI context).
    （QSAサイクルの特定の側面や単純なループを示す、簡潔で自己完結した例（潜在的にSUIコンテキスト内で）。）
-   **`/docs/case-studies/`:** Detailed, multi-loop explorations applying the SUI/QSA approach to specific problems, showcasing recursive power and interaction patterns.
    （特定の課題に SUI/QSA アプローチを適用し、その再帰的な力や相互作用パターンを示す、詳細で複数ループにわたる探求。）

---

## Standard Document Structure / 標準文書構成

Each document must begin with a YAML front matter block including these core fields:
各文書は、以下のコアフィールドを含むYAMLフロントマターから始める必要があります。

```yaml
---
title: "Title of the Document / ドキュメントタイトル"
description: "Brief summary (2–3 lines) / ドキュメント概要（2〜3行）"
target_audience: ["LLM", "Human"] # Add others like Researcher, Developer, Contributor as needed
document_type: "Concept | Research | Comparison | Extension | Example | CaseStudy | Guide | Other" # ★タイプ追加
tags: ["SUI", "QSA", "Specific_Topic"] # Add relevant tags reflecting content
status: "draft | published | revised"
created_at: "YYYY-MM-DD" # Date of first commit/creation
updated_at: "YYYY-MM-DD" # Date of last significant revision
license: "MIT"
language: ["en", "ja"]
---
```

*Optional fields like `version`, `related`, `keywords`, `contributors`, `audience_level`, `scope/focus` can be added for enhanced metadata if necessary.*
*（必要に応じて、メタデータを強化するために `version`, `related`, `keywords`, `contributors`, `audience_level`, `scope/focus` などの任意項目を追加可能です。）*

Followed by structured Markdown content. While specific sections may vary by `document_type`, common useful sections include:
続いて、構造化されたMarkdown本文を記述します。`document_type` によって特定のセクションは異なる場合がありますが、一般的に有用なセクションは次のとおりです。

-   `Purpose / 目的`
-   `Overview / 概要` or `Introduction / はじめに`
-   `Core Content / コアコンテンツ` (Potentially broken into Q/S/A/T for QSA examples/case studies)
    （QSAの例やケーススタディでは Q/S/A/T に分割される可能性あり）
-   `Key Takeaways / 要点` or `Conclusion / 結論`
-   `Related Documents / 関連ドキュメント` (Optional)
-   `Future Work / 今後の課題` (Optional)

---

## Template / テンプレート

A master template reflecting this structure is provided at [`template.md`](./template.md).
この構造を反映したマスターテンプレートは [`template.md`](./template.md) に用意されています。

---

## Contribution Guide / 貢献ガイド

When creating a new document:
（新しいドキュメントを作成する際は、以下に従ってください。）

1.  Copy `template.md` and rename it appropriately (e.g., `sui-interaction-patterns.md`).
    （`template.md` をコピーし、適切にリネームします（例：`sui-interaction-patterns.md`）。）
2.  Place it in the relevant subdirectory (`/concepts`, `/research`, `/extensions`, `/examples`, `/case-studies`).
    （関連するサブディレクトリ（`/concepts`, `/research`, `/extensions`, `/examples`, `/case-studies`）に配置します。）
3.  Fill in the YAML metadata accurately, paying close attention to `title`, `description`, `document_type`, `tags`, and dates. Use descriptive tags reflecting SUI/QSA and the specific topic.
    （YAMLメタデータを正確に記入します。特に`title`, `description`, `document_type`, `tags`, 日付に注意してください。SUI/QSAおよび特定のトピックを反映する内容をよく表すタグを使用します。）
4.  Structure the content logically. For QSA examples/case studies, explicitly using the Q/S/A/T structure is highly recommended. For SUI discussions, clearly define relevant semantic primitives.
    （内容を論理的に構成します。QSAの例やケーススタディでは、Q/S/A/T 構造を明示的に使用することを強く推奨します。SUIの議論では、関連する意味的プリミティブを明確に定義します。）
5.  Write with **both LLM processability and human clarity in mind**, reflecting the SUI/QSA co-thinking philosophy. Use clear headings, lists (using `-` followed by a space), and potentially code blocks for structure. Indent lists with two spaces. Adhere to Markdown formatting rules specified in the main project `README.md`.
    （**LLMによる処理可能性と人間にとっての明瞭性の両方を念頭に置いて**執筆し、SUI/QSAの共同思考の哲学を反映させます。明確な見出し、リスト（`-` の後にスペース）、そして構造を示すためのコードブロックを効果的に使用します。リストのインデントはスペース2つで行います。メインプロジェクトの`README.md`で指定されたMarkdown書式ルールに従ってください。）

---

## Notes / 注意事項

-   Always update the `updated_at` field upon significant revision.
    （大幅な改訂時には必ず`updated_at`フィールドを更新してください。）
-   Use tags consistently for findability and potential automation.
    （発見可能性と潜在的な自動化のためにタグを一貫して使用してください。）
-   Maintain the bilingual (`en`, `ja`) format where applicable.
    （該当する場合はバイリンガル（`en`, `ja`）形式を維持してください。）
-   Strive for clarity and precision, suitable for explaining concepts and potentially serving as input/output within SUI/QSA processes.
    （概念を説明するため、そして潜在的には SUI/QSA プロセス自体の入出力としても機能するのに適した、明確さと正確さを追求してください。）


---

## QSA Loop Recording Template / QSAループ記録用テンプレート

For documenting specific QSA execution cycles, particularly within `docs/examples/` and `docs/case-studies/` (e.g., files named `loop-xx_*.md`), a dedicated QSA loop recording template should be used. This template is designed to capture the iterative thinking process.
（特定のQSA実行サイクルを記録する場合、特に `docs/examples/` や `docs/case-studies/` 内のファイル（例：`loop-xx_*.md` という名前のファイル）については、専用のQSAループ記録用テンプレートを使用します。このテンプレートは、反復的な思考プロセスを捉えるために設計されています。）

The general structure of this template is:
（このテンプレートの一般的な構造は次のとおりです：）

```yaml
---
title: "(LLMが生成 or 手動設定)"
created_at: "(LLMが生成 or 手動設定)"
tags: [QSA, (relevant_tags)]
# Other optional YAML keys: description, target_audience, document_type (e.g., "QSA Loop Log"), status, updated_at, license, language, qsa_loop_id, case_study_id, etc.
---

## Context / 背景・きっかけ
* (Why this QSA loop was started, origin, links to related notes, etc.)

## References / 関連メモ・リンク
* (List of internal/external links related to this cycle.)

## Thinking Log / 思考ログ

### Q (Question)
* (The central question for this cycle.)

### S (Structure)
* (Design of the thinking structure to answer Q: decomposition, comparison axes, framework, assumptions, etc.)

### A (Answer)
* (The response derived based on the structure S: hypotheses, analysis results, partial conclusions, discoveries, etc.)

### T (Thought)
* (Reflection on A, evaluation, and connections to the next thought cycle: validity of A, new questions, next steps.)

## Distillation (Optional)
* (Core insights, conclusions, key discoveries, next concrete actions, or seeds for output extracted from this QSA cycle.)


```

Refer to actual examples in `docs/examples/` for practical application. For general conceptual documents, guides, or research papers, continue to use the main `template.md` as a base.
（実際の適用例については `docs/examples/` 内の例を参照してください。一般的な概念ドキュメント、ガイド、研究論文については、引き続きメインの `template.md` をベースとして使用してください。）
