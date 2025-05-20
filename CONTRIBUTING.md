---
title: "Contribution Guidelines / 貢献ガイドライン"
description: "Guidelines for contributing to the SUI & QSA Model repository, including documentation standards, QSA loop recording, and general best practices. / SUIおよびQSAモデルリポジトリへの貢献に関するガイドライン。ドキュメント標準、QSAループ記録方法、一般的なベストプラクティスを含む。"
target_audience: ["Contributor", "Developer", "Researcher"]
document_type: "Guide"
tags: ["Contribution", "Style Guide", "Documentation", "QSA", "SUI", "Templates"]
status: "draft"
created_at: "2025-05-21"
updated_at: "2025-05-21"
license: "MIT"
language: ["ja", "en"]
---

# Contribution Guidelines / 貢献ガイドライン

Thank you for your interest in contributing to the SUI & QSA Model repository! Your contributions can help improve the clarity, depth, and applicability of these concepts for human-AI co-thinking.
（SUIおよびQSAモデルリポジトリへの貢献にご関心をお寄せいただきありがとうございます！あなたの貢献は、人間とAIの共同思考のためのこれらの概念の明確さ、深さ、そして適用可能性を向上させるのに役立ちます。）

## Core Philosophy / コアとなる哲学

This repository aims to explore and document the **SUI (Semantic User Interface) paradigm** and the **QSA (Question → Structure → Answer → Thought) model**. All contributions should align with the core philosophy of enhancing human-AI collaboration, grounded in a cyclical view of intelligence (see [`docs/00_overview/philosophy_of_intelligence.md`](./docs/00_overview/philosophy_of_intelligence.md)).
（本リポジトリは、**SUI（意味的ユーザーインターフェース）パラダイム**および**QSA（問い→構造→答え→思考）モデル**を探求し文書化することを目的としています。すべての貢献は、知性の循環的視点（[`docs/00_overview/philosophy_of_intelligence.md`](./docs/00_overview/philosophy_of_intelligence.md)参照）に基づいた、人間とAIの協調を強化するというコアフィロソフィーに沿うべきです。）

## Documentation Standards / ドキュメント標準

All documents in the `docs/` directory should adhere to the following standards to ensure consistency and readability for both humans and LLMs.
（`docs/`ディレクトリ内のすべてのドキュメントは、人間とLLM双方にとっての一貫性と可読性を確保するために、以下の標準に準拠する必要があります。）

### 1. YAML Frontmatter / YAMLフロントマター

Each document must begin with a YAML front matter block.
（各ドキュメントはYAMLフロントマターブロックで始まる必要があります。）

-   **Required Fields / 必須フィールド:**
    ```yaml
    ---
    title: "Descriptive Title / 分かりやすいタイトル"
    description: "Brief summary (1-2 sentences) of the document's content. / 内容の簡潔な要約（1～2文）。"
    target_audience: ["LLM", "Human", "Researcher", "Developer", "Practitioner", "Contributor", "Manager", "Leader", "Executive", "Student", "Learner", "Philosopher", "Designer", "Implementer"] # Choose all relevant
    document_type: "Overview | Concept | Guide | Research | Comparison | Extension | Example | CaseStudy | QSALoopRecord | AnalysisLoop | AnalysisSummary | Briefing Paper | Article | Workshop Materials | Other" # Choose one primary type
    tags: ["SUI", "QSA", "ZLD", "IPS", "Specific_Topic1", "Specific_Topic2"] # Include SUI/QSA/ZLD/IPS and other relevant topic tags
    status: "draft | published | revised | obsoleted" # Current status
    created_at: "YYYY-MM-DD" # Date of first commit/creation
    updated_at: "YYYY-MM-DD" # Date of last significant revision
    license: "MIT"
    language: ["ja", "en"] # Primary language first if bilingual
    ---
    ```
-   **Optional Fields / 任意フィールド (as needed):**
    ```yaml
    version: "X.Y" # For versioned documents
    related: # Links to related documents (relative paths)
      - ../another_folder/related_document.md
    qsa_loop_id: "unique-loop-identifier" # For QSA loop records
    case_study_id: "unique-case-study-id" # For case studies
    dependencies: [qsa_loop_id_of_previous_loop] # For QSA loops
    next_loop_candidates: # For QSA loops
      - qsa_loop_id_for_next_1
      - qsa_loop_id_for_next_2
    source_conversation_context: "Brief description of the LLM conversation or source material" # For documents derived from specific interactions
    source_deep_research_link: "URL to LLM conversation if applicable"
    # Add other custom fields relevant to the document type
    ```

### 2. Markdown Formatting / Markdownフォーマット

Please follow the guidelines in [`250512_markdown-style-guide-jp.md`](./250512_markdown-style-guide-jp.md) for consistent Markdown usage. Key points include:
（一貫したMarkdownの使用については、[`250512_markdown-style-guide-jp.md`](./250512_markdown-style-guide-jp.md) のガイドラインに従ってください。主なポイントは以下の通りです。）

-   Lists: Use `-` with a single space, indent with 2 spaces for nesting.
    （リスト：`-` を使用し、半角スペース1つ。ネストは半角スペース2つでインデント。）
-   Headings: Start from `##` (H2), step down one level at a time.
    （見出し：`##`（H2）から開始し、1レベルずつ下げる。）
-   Emphasis: Use `**bold**` sparingly. Avoid italics or strikethrough. Pay attention to full-width characters with emphasis.
    （強調：`**太字**` は最小限に。斜体や打ち消し線は使用しない。全角文字と強調の扱いに注意。）

### 3. Document Structure / ドキュメント構造

While specific sections may vary by `document_type`, strive for logical flow and clarity. Common useful sections include:
（`document_type` によって特定のセクションは異なりますが、論理的な流れと明確さを心がけてください。一般的に有用なセクションは次のとおりです。）

-   `## Purpose / 目的`
-   `## Overview / 概要` or `## Introduction / はじめに`
-   `## Core Content / コアコンテンツ` (or specific QSA sections)
-   `## Key Takeaways / 要点` or `## Conclusion / 結論`
-   `## Related Documents / 関連ドキュメント` (Optional)
-   `## Future Work / 今後の課題` (Optional)

### 4. LLM Interpretation Guidelines / LLMによる解釈のためのガイドライン

(このセクションには、以前 `docs/20_qsa/README.md` にあった「Guidelines for LLM Interpretation」の内容を移管・統合します。SとAの区別、LLM処理の提案など。)
```
To ensure accurate understanding and application of the QSA model and related concepts by Large Language Models (LLMs), please adhere to the following interpretations, especially regarding the distinction between **Structure (S)** and **Answer (A)** phases:

1.  **Role of Structure (S):**
    *   The S phase is dedicated to defining the **methodology, plan, framework, or outline** for how to approach and answer the given Question (Q).
    *   It involves activities like decomposing the question, identifying key areas of inquiry, establishing analytical steps, or setting up a logical flow for reasoning.
    *   **Crucially, S does NOT contain the direct answer, conclusion, or specific solution to Q.** It is the blueprint for generating the answer, not the answer itself. Think of it as the "recipe" or "architectural plan."
    *   Refer to `docs/00_overview/concept_overview.md` for a detailed definition of S.

    （**構造（S）の役割：**）
    *   （Sフェーズは、与えられた問い（Q）にどのようにアプローチし、どのように答えるかという**方法論、計画、フレームワーク、または骨子**を定義することに専念します。）
    *   （問いの分解、主要な探求領域の特定、分析ステップの確立、推論のための論理的な流れの設定などの活動を含みます。）
    *   （**重要な点として、SはQに対する直接的な答え、結論、または具体的な解決策を含みません。** これは答えを生成するための設計図であり、答えそのものではありません。「レシピ」や「建築計画」と考えてください。）
    *   （Sの詳細な定義については `docs/00_overview/concept_overview.md` を参照してください。）

2.  **Role of Answer (A):**
    *   The A phase involves generating the **specific content, analysis, findings, or response** to Q, strictly following the methodology, plan, or framework established in S.
    *   It is the **execution** of the plan laid out in S.
    *   If S outlines "how to answer," A provides "the actual answer."
    *   Refer to `docs/00_overview/concept_overview.md` for a detailed definition of A.

    （**答え（A）の役割：**）
    *   （Aフェーズは、Sで確立された方法論、計画、またはフレームワークに厳密に従い、Qに対する**具体的な内容、分析、発見、または応答**を生成することを含みます。）
    *   （これはSで提示された計画の**実行**です。）
    *   （Sが「どのように答えるか」を概説する場合、Aは「実際の答え」を提供します。）
    *   （Aの詳細な定義については `docs/00_overview/concept_overview.md` を参照してください。）

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
```

## Using Templates / テンプレートの使用

This repository provides two main templates located in the [`templates/`](./templates/) directory:
（本リポジトリでは、[`templates/`](./templates/) ディレクトリに2つの主要なテンプレートを提供しています。）

1.  **[`templates/qsa_loop_template.md`](./templates/qsa_loop_template.md):**
    -   **Purpose:** For recording specific QSA execution cycles, typically used for documents within `docs/examples/` and `docs/50_case-studies/` (e.g., files named `loop-xx_*.md`).
        （**目的：** 特定のQSA実行サイクルを記録するため。通常、`docs/examples/` および `docs/50_case-studies/` 内のドキュメント（例：`loop-xx_*.md` という名前のファイル）に使用します。）
    -   **Structure:** Includes YAML frontmatter presets and sections for `Context`, `References`, `Thinking Log (Q, S, A, T)`, and `Distillation (Optional)`.
        （**構造：** YAMLフロントマターのプリセットと、`Context`、`References`、`Thinking Log (Q, S, A, T)`、および `Distillation (Optional)` のセクションを含みます。）
    -   **Usage:** Copy this template when starting a new QSA loop analysis or documenting a specific thinking process iteration. Fill in the YAML fields and Markdown sections accordingly.
        （**使用法：** 新しいQSAループ分析を開始する際や、特定の思考プロセスの反復を文書化する際に、このテンプレートをコピーしてください。YAMLフィールドとMarkdownセクションを適宜記入します。）

2.  **[`templates/repository_document_template.md`](./templates/repository_document_template.md):**
    -   **Purpose:** A general-purpose template for creating conceptual explanations, guides, research papers, comparisons, or other non-QSA-loop-specific documents within the `docs/` directory.
        （**目的：** `docs/` ディレクトリ内に、概念説明、ガイド、研究論文、比較、その他QSAループ特有ではない一般的なドキュメントを作成するための汎用テンプレート。）
    -   **Structure:** Includes a comprehensive YAML frontmatter preset and suggested Markdown sections like `Purpose`, `Overview`, `Core Content`, `Key Takeaways`, etc.
        （**構造：** 包括的なYAMLフロントマターのプリセットと、`Purpose`、`Overview`、`Core Content`、`Key Takeaways` などの推奨Markdownセクションを含みます。）
    -   **Usage:** Use this as a starting point for any new document that is not a direct record of a QSA cycle. Adapt the sections as needed for the specific `document_type`.
        （QSAサイクルの直接的な記録ではない新しいドキュメントの開始点として使用してください。特定の `document_type` に合わせてセクションを適宜変更します。）

## General Contribution Process (Future) / 一般的な貢献プロセス（将来的に）

While this repository is currently primarily managed by the initial author, we envision a future where community contributions are welcomed. When that time comes, the process will likely involve:
（現在、本リポジトリは主に初期作成者によって管理されていますが、将来的にはコミュニティからの貢献を歓迎することを想定しています。その際には、以下のようなプロセスになる可能性があります。）

1.  **Discuss:** Propose your idea or change in a GitHub Issue first.
    （まずGitHub Issueでアイデアや変更を提案してください。）
2.  **Fork:** Fork the repository.
    （リポジトリをフォークしてください。）
3.  **Branch:** Create a new branch for your changes.
    （変更のために新しいブランチを作成してください。）
4.  **Develop:** Make your changes, adhering to the documentation and style guidelines.
    （ドキュメンテーションおよびスタイルガイドラインに従って変更を加えてください。）
5.  **Test:** Ensure your changes are clear, accurate, and well-formatted.
    （変更が明確、正確、かつ適切にフォーマットされていることを確認してください。）
6.  **Pull Request:** Submit a Pull Request with a clear description of your contribution.
    （貢献内容を明確に記述したプルリクエストを送信してください。）

Thank you for helping to build a valuable resource for advancing human-AI co-thinking!
（人間とAIの共同思考を前進させるための貴重なリソース構築にご協力いただきありがとうございます！）
