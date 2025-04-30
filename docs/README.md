---
title: "Documentation Guide for QSA Model / QSAモデル文書化ガイド"
description: "Provides guidelines and standards for creating and organizing documentation within the QSA Model repository, ensuring consistency and readability for both humans and LLMs. / QSAモデルリポジトリ内のドキュメント作成・整理に関するガイドラインと標準を提供し、人間とLLM双方にとっての一貫性と可読性を確保します。"
target_audience: ["Contributor", "LLM", "Human", "Researcher"] # Contributorを追加
document_type: "Guide" # タイプをGuideに変更
tags: ["QSA", "Documentation", "Contribution Guide", "Metadata", "Standards", "YAML", "Markdown"] # タグを追加・修正
status: "published" # publishedに変更 (ガイドとして)
created_at: "2025-04-27" # 元ファイルの作成日を維持 (仮)
updated_at: "2025-05-01" # 更新日 (仮)
license: "MIT"
language: ["en", "ja"]
---

# Documentation Guide for QSA Model / QSAモデル文書化ガイド

---

## Overview / 概要

This `docs/` directory serves as the central knowledge base for the **QSA Model (Question → Structure → Answer → Thought)**. It contains conceptual explanations, comparisons with existing models, practical examples, **in-depth case studies demonstrating the model in action**, and research validating its originality.

この `docs/` ディレクトリは、**QSAモデル（問い→構造→答え→思考）**の中心的なナレッジベースとして機能します。ここには、概念説明、既存モデルとの比較、実用例、**モデルの実践を示す詳細なケーススタディ**、そしてその独自性を検証する調査が含まれます。

All documents adhere to a standard structure designed to be optimally processed by **LLMs** and easily understood by **human readers**, reflecting the **human-AI collaborative nature** of the QSA model itself.

すべての文書は、**LLM** による最適な処理と**人間読者**による容易な理解のために設計された標準構成に従っています。これは、QSAモデル自体の**人間-AI協働という性質**を反映しています。

---

## Directory Structure / ディレクトリ構造

- **`/docs` (root):** Core documents like this guide, the concept overview, comparisons, originality research, and the template.
    （このガイド、コンセプト概要、比較、独自性調査、テンプレートなどのコアドキュメント。）
- **`/docs/examples/`:** Contains **concise, self-contained examples** illustrating specific aspects or simple loops of the QSA cycle.
    （QSAサイクルの特定の側面や単純なループを示す、**簡潔で自己完結した例**を含みます。）
- **`/docs/case-studies/`:** Houses **detailed, multi-loop explorations** applying the QSA model to specific problems or questions, showcasing its recursive power and human-AI interaction patterns. (e.g., Text File Evolution study).
    （特定の課題や問いに QSA モデルを適用し、その再帰的な力や人間-AIインタラクションのパターンを示す、**詳細で複数ループにわたる探求**を格納します。（例：テキストファイル進化の研究））
- **`/docs/extensions/` (Potentially):** Might contain documents describing extensions or related frameworks like iPS. *(Current recommendation: Move iPS Framework here for better organization)*
    （iPSのような拡張機能や関連フレームワークを説明するドキュメントを含む可能性があります。（現在の推奨：より良い整理のため、iPSフレームワークをここに移動）)* # コメントを少し具体化

---

## Standard Document Structure / 標準文書構成

Each document must begin with a YAML front matter block including these core fields:
各文書は、以下のコアフィールドを含むYAMLフロントマターから始める必要があります。

```yaml
---
title: "Title of the Document / ドキュメントタイトル"
description: "Brief summary (2–3 lines) / ドキュメント概要（2〜3行）"
target_audience: ["LLM", "Human"] # Add others like Researcher, Developer, Contributor as needed
document_type: "Concept | Comparison | Example | CaseStudy | Extension | Guide | Other" # CaseStudy, Guideを追加
tags: ["QSA", "LLM Reasoning", "Specific_Topic"] # Add relevant tags reflecting content
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

- `Purpose / 目的`
- `Overview / 概要` or `Introduction / はじめに`
- `Core Content / コアコンテンツ` (Potentially broken into Q/S/A/T for examples/case studies)
    （例やケーススタディでは Q/S/A/T に分割される可能性あり）
- `Key Takeaways / 要点` or `Conclusion / 結論`
- `Related Documents / 関連ドキュメント` (Optional)
- `Future Work / 今後の課題` (Optional)

---

## Template / テンプレート

A master template reflecting this structure is provided at [`docs/template.md`](./template.md).
この構造を反映したマスターテンプレートは [`docs/template.md`](./template.md) に用意されています。

When creating a new document:
新しいドキュメントを作成する際は、以下に従ってください。

1. Copy `template.md` and rename it appropriately (e.g., `qsa-for-research.md`).
    `template.md` をコピーし、適切にリネームします（例：`qsa-for-research.md`）。
2. Place it in the relevant subdirectory (`/examples`, `/case-studies`, `/extensions`, etc.).
    関連するサブディレクトリ（`/examples`, `/case-studies`, `/extensions` など）に配置します。
3. Fill in the YAML metadata accurately, paying close attention to `title`, `description`, `document_type`, `tags`, and dates. Use descriptive tags.
    YAMLメタデータを正確に記入します。特に`title`, `description`, `document_type`, `tags`, 日付に注意してください。内容をよく表すタグを使用します。
4. Structure the content logically. For examples and case studies, explicitly using the Q/S/A/T structure within the `Core Content` section is highly recommended.
    内容を論理的に構成します。例やケーススタディでは、「コアコンテンツ」セクション内で Q/S/A/T 構造を明示的に使用することを強く推奨します。
5. Write with **both LLM processability and human clarity in mind**, reflecting the QSA's co-thinking philosophy. Use clear headings, lists (using `-` followed by a space), and potentially code blocks for structure (like in the S phase). Indent lists with two spaces.
    **LLMによる処理可能性と人間にとっての明瞭性の両方を念頭に置いて**執筆し、QSAの共同思考の哲学を反映させます。明確な見出し、リスト（`-` の後にスペース）、そして構造を示すためのコードブロック（Sフェーズのように）を効果的に使用します。リストのインデントはスペース2つで行います。 # Markdownルール追記

---

## Notes / 注意事項

- Always update the `updated_at` field upon significant revision.
    大幅な改訂時には必ず`updated_at`フィールドを更新してください。
- Use tags consistently for findability and potential automation. Consider adding specific topic tags (e.g., `Markdown`, `Adoption Strategy`).
    発見可能性と潜在的な自動化のためにタグを一貫して使用してください。特定のトピックタグ（例：`Markdown`, `Adoption Strategy`）の追加を検討してください。
- Maintain the bilingual (`en`, `ja`) format where applicable.
    該当する場合はバイリンガル（`en`, `ja`）形式を維持してください。
- Strive for clarity and precision, suitable for both explaining a concept and potentially serving as input/output within a QSA process itself. Ensure adherence to Markdown formatting rules (e.g., lists with `-`).
    概念を説明するため、そして潜在的には QSA プロセス自体の入出力としても機能するのに適した、明確さと正確さを追求してください。Markdownの書式ルール（例：`-`を使ったリスト）の遵守を徹底してください。 # Markdownルール遵守を追記

---
