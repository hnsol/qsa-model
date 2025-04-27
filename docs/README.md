# Documentation Guide for QSA Model / QSAモデル文書化ガイド

---

## Overview / 概要

This `docs/` directory contains conceptual explanations, comparisons with existing models, and practical examples related to the QSA Model (Question → Structure → Answer → Thought).

この `docs/` ディレクトリには、QSAモデル（問い→構造→答え→思考）に関連する概念説明、既存モデルとの比較、実用例が含まれます。

All documents follow a standard structure designed to be readable by both LLMs and human readers.

すべての文書は、LLMと人間読者の両方にとって可読性の高い標準構成に従っています。

---

## Standard Document Structure / 標準文書構成

Each document must begin with a YAML front matter block including:  
各文書は、以下のYAMLフロントマターから始める必要があります。

```yaml
---
title: "Title of the Document / ドキュメントタイトル"
description: "Brief summary (2–3 lines) / ドキュメント概要（2〜3行）"
target_audience: ["LLM", "Human"]
document_type: "Concept | Comparison | Example | Extension | Other"
tags: ["QSA", "LLM Reasoning"]
status: "draft" # または "published", "revised"
created_at: "YYYY-MM-DD"
updated_at: "YYYY-MM-DD"
license: "MIT"
language: ["en", "ja"]
---
```

Followed by structured Markdown content organized into sections like:  
続いて、以下のようなセクションで構成されたMarkdown本文を記述します。

- `Purpose / 目的`
- `Core Content / コアコンテンツ`
- `Key Points / 重要ポイント`
- `Related Topics (optional) / 関連トピック（任意）`
- `Future Work (optional) / 将来展望（任意）`

---

## Template / テンプレート

A master template is provided at [`docs/template.md`](./template.md).  
マスターテンプレートは [`docs/template.md`](./template.md) に用意されています。

When creating a new document:  
新しいドキュメントを作成する際は、以下に従ってください。

1. Copy `template.md` and rename it appropriately.  
   `template.md` をコピーし、適切なファイル名にリネームします。
2. Fill in the YAML metadata carefully, especially `title`, `description`, `document_type`, and dates.  
   YAMLメタデータを丁寧に記入します（特に`title`、`description`、`document_type`、日付）。
3. Structure your main content following the guidelines.  
   ガイドラインに沿って本文を構成します。
4. Keep a clear, recursive thinking cycle in mind, suitable for both LLM parsing and human understanding.  
   LLMの解析および人間の理解に適した、明確な再帰的思考サイクルを意識します。

---

## Notes / 注意事項

- Always update the `updated_at` field when revising a document.  
  ドキュメントを改訂した際は、必ず`updated_at`フィールドを更新してください。
- Ensure consistent use of tags for easier future indexing and automatic processing.  
  将来的な索引化や自動処理を容易にするため、タグの使用を一貫させてください。
- Keep both machine readability and human readability in mind.  
  機械可読性と人間可読性の両方を意識してください。

---
