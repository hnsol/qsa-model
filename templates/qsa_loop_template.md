
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
