# Documentation Guide for QSA Model

## Overview

This `docs/` directory contains conceptual explanations, comparisons with existing models, and practical examples related to the QSA Model (Question → Structure → Answer → Thought).

All documents follow a standard structure designed to be readable by both LLMs and human readers.

## Standard Document Structure

Each document must begin with a YAML front matter block including:

```yaml
---
title: "Title of the Document"
description: "Brief summary (2–3 lines)"
target_audience: ["LLM", "Human"]
document_type: "Concept | Comparison | Example | Extension | Other"
tags: ["QSA", "LLM Reasoning"]
status: "draft" # or "published", "revised"
created_at: "YYYY-MM-DD"
updated_at: "YYYY-MM-DD"
license: "MIT"
---
```

Followed by structured Markdown content organized into sections like:

- `Purpose`
- `Core Content`
- `Key Points`
- `Related Topics (optional)`
- `Future Work (optional)`

## Template

A master template is provided at [`docs/template.md`](./template.md).

When creating a new document:
1. Copy `template.md` and rename it appropriately.
2. Fill in the YAML metadata carefully, especially `title`, `description`, `document_type`, and dates.
3. Structure your main content following the guidelines.
4. Keep a clear, recursive thinking cycle in mind, suitable for both LLM parsing and human understanding.

## Notes

- Always update the `updated_at` field when revising a document.
- Ensure consistent use of tags for easier future indexing and automatic processing.
- Keep both machine readability and human readability in mind.
