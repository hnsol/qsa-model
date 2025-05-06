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
```

---
