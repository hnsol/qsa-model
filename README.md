---
title: "QSA Model & SUI Paradigm - Human-AI Co-Thinking Framework / QSAモデルとSUIパラダイム - 人間とAIの共同思考フレームワーク"
description: "The QSA (Question → Structure → Answer → Thought) Model: A structured protocol operating within the SUI (Semantic User Interface) paradigm, designed to enhance human-AI collaborative reasoning and cognitive evolution, **grounded in a cyclical view of intelligence as information compression and meaning expansion.** / QSAモデル（問い→構造→答え→思考）：SUI（意味的ユーザーインターフェース）パラダイム内で動作する構造化プロトコル。人間とAIの協調的推論と認知的進化を強化するために設計。**知的情報の圧縮と意味の展開という循環的な知性観に立脚。**"
target_audience: ["LLM", "Human", "Researcher", "Developer"]
document_type: "Overview"
tags: ["QSA", "SUI", "ZLD", "IPS", "LLM Reasoning", "Human-AI Collaboration", "Co-Thinking", "Cognitive Evolution", "Structured Thought", "Cognitive Protocol", "AI Interface", "Interaction Paradigm", "Quaerentes", "Intelligence", "Compression", "Expansion", "Knowledge Management"]
status: "published"
created_at: "2025-04-27"
updated_at: "2025-05-21" # 更新
license: "MIT"
language: ["ja", "en"]
---

# QSA Model & SUI Paradigm - Empowering Human-AI Co-Thinking / QSAモデルとSUIパラダイム - 人間とAIの共同思考を強化する

> Structuring the Future of Human-AI Collaboration, **Rooted in a New Understanding of Intelligence** / 人間とAIの協働が生み出す未来を構造化する、**知性の新たな理解に根ざして**

---

## Why: なぜこのリポジトリなのか？ (目的と背景)

現代は情報が爆発的に増加し、AI、特に大規模言語モデル（LLM）が人間の知的活動のあらゆる側面に浸透しつつあります。このような時代において、人間とAIが真に協調し、より深い洞察や創造的な解決策を生み出すためには、**思考のプロセスそのものを構造化し、共有するための新しい枠組み**が不可欠です。

本リポジトリは、この課題意識に基づき、**「知性は情報の圧縮と意味の展開の循環である」** という独自の哲学的視点（詳細は [`docs/00_overview/philosophy_of_intelligence.md`](./docs/00_overview/philosophy_of_intelligence.md) 参照）から、人間とAIの協調的推論と認知的進化を強化するための一連の概念とプロトコルを提案します。

## What: 何が学べるのか・何があるのか？ (主要概念とドキュメント構成)

本リポジトリでは、以下の主要な概念を探求し、その実践方法を提示します。

1.  **SUI (Semantic User Interface) Paradigm / SUIパラダイム:**
    -   人間とAIの共同思考のための基本的な対話パラダイム。意味と構造を中心としたインタラクションを目指します。
    -   詳細は [`docs/10_sui/README.md`](./docs/10_sui/README.md) および [`docs/10_sui/sui_concept.md`](./docs/10_sui/sui_concept.md) を参照。
2.  **QSA (Question → Structure → Answer → Thought) Model / QSAモデル:**
    -   SUIパラダイム内で動作する、構造化された再帰的な認知プロトコル。問いを起点に、人間とAIが協調して理解と洞察を進化させるワークフローです。
    -   導入と実践については [`docs/20_qsa/README.md`](./docs/20_qsa/README.md) を、核心的な概念については [`docs/00_overview/concept_overview.md`](./docs/00_overview/concept_overview.md) を参照。
3.  **IPS (Intent → Plan → Scope) Framework / IPSフレームワーク:**
    -   QSAモデルの「Structure（構造）」フェーズを効果的に設計するための軽量ガイドライン。
    -   詳細は [`docs/30_qsa_extensions/README.md`](./docs/30_qsa_extensions/README.md) および [`docs/30_qsa_extensions/ips_framework.md`](./docs/30_qsa_extensions/ips_framework.md) を参照。
4.  **ZLD (Zetteldistillat) / ツェッテルディスティラート:**
    -   SUIパラダイムの一つの具体的な実装例であり、QSAモデルを個々の知識要素（ツェッテル）の構成と思考の精製・蒸留プロセスに応用するアプローチ。
    -   詳細は [`docs/40_implementations/README.md`](./docs/40_implementations/README.md) および [`docs/40_implementations/zld/loop-04_zd-core-principles.md`](./docs/40_implementations/zld/loop-04_zd-core-principles.md) を参照。

これらの概念の関係性や全体像については、[`docs/00_overview/README.md`](./docs/00_overview/README.md) にある**概念マップ**も参照してください。

## How: どう読み進めるか・どう使うか？ (歩き方)

1.  **全体像の把握:** まずはこの `README.md` を通読し、次に [`docs/00_overview/README.md`](./docs/00_overview/README.md) とそこにある概念マップで全体像を掴んでください。我々の根底にある思想については [`docs/00_overview/philosophy_of_intelligence.md`](./docs/00_overview/philosophy_of_intelligence.md) が参考になります。
2.  **主要概念の理解:**
    -   SUIパラダイムに興味があれば [`docs/10_sui/sui_concept.md`](./docs/10_sui/sui_concept.md) を。
    -   QSAモデルの核心を知りたければ [`docs/00_overview/concept_overview.md`](./docs/00_overview/concept_overview.md) を、その実践的側面については [`docs/20_qsa/README.md`](./docs/20_qsa/README.md) をお読みください。
3.  **QSAを実践する:**
    -   QSAループの具体的なテンプレートは [`templates/qsa_loop_template.md`](./templates/qsa_loop_template.md) にあります。
    -   実践的なサンプルは [`examples/`](./examples/) フォルダ内にあります。（例: [`examples/simple_loop_example.md`](./examples/simple_loop_example.md)）
4.  **より深く探求する:**
    -   QSAの拡張（IPSフレームワーク）や実装例（Zetteldistillat）、詳細なケーススタディ、独自性に関する調査は、それぞれ `docs/` 配下の各フォルダに格納されています。各フォルダの `README.md` が案内役となります。

---

## Priority Claim / 優先公開宣言

This repository establishes the initial public disclosure of:
（本リポジトリは、以下について初めて一般に公開したことを証明するものです。）

-   The **QSA Model** (Question → Structure → Answer → Thought) as a structured, recursive cognitive protocol for human-AI co-thinking (as of `2025-04-27`).
    （QSAモデル（問い→構造→答え→思考）：人間とAIの共同思考のための構造化された再帰的認知プロトコル（`2025-04-27`付）。）
-   The **SUI (Semantic User Interface) Paradigm** as a fundamental interaction paradigm for human-AI co-thinking, especially when understood through its foundational philosophy of cyclical intelligence (compression-expansion) (conceptualized around `2025-05-02`).
    （SUI（意味的ユーザーインターフェース）パラダイム：人間とAIの共同思考のための基本的な相互作用パラダイム。特に、その循環的知性（圧縮と展開）という基盤哲学を通じて理解される場合（`2025-05-02`頃概念化）。）

Furthermore, this repository explores and proposes unique interpretations and practical applications of:
（さらに、本リポジトリは以下の独自の解釈と実践的応用を探求・提案します。）

-   The **Zetteldistillat (ZLD)** approach as an implementation of SUI/QSA for knowledge distillation (details in [`docs/40_implementations/zld/loop-04_zd-core-principles.md`](./docs/40_implementations/zld/loop-04_zd-core-principles.md)).
    （Zetteldistillat（ZLD）アプローチ：知識蒸留のためのSUI/QSAの実装例（詳細は [`docs/40_implementations/zld/loop-04_zd-core-principles.md`](./docs/40_implementations/zld/loop-04_zd-core-principles.md) 参照）。）
-   The **iPS Framework** (Intent → Plan → Scope) as a method for designing the Structure (S) phase of QSA (details in [`docs/30_qsa_extensions/ips_framework.md`](./docs/30_qsa_extensions/ips_framework.md)).
    （iPSフレームワーク（インテント→プラン→スコープ）：QSAの構造（S）フェーズを設計するための手法（詳細は [`docs/30_qsa_extensions/ips_framework.md`](./docs/30_qsa_extensions/ips_framework.md) 参照）。）

The novelty lies in **systematically formalizing these concepts and their interrelations as an operational protocol and interaction paradigm specifically designed to facilitate effective human-AI cognitive collaboration and synergy, based on an explicit model of how intelligence processes information.**
（新規性は、**知性が情報を処理する方法に関する明示的なモデルに基づき、これらの概念とその相互関係を、人間とAIの効果的な認知的協働と相乗効果を促進するために特別に設計された運用可能なプロトコルおよびインタラクションパラダイムとして体系的に定式化した点**にあります。）

Detailed research on originality and comparisons can be found in:
（独自性と比較に関する詳細な調査は以下にあります。）
-   [`docs/10_sui/sui_originality.md`](./docs/10_sui/sui_originality.md)
-   [`docs/20_qsa/qsa_originality.md`](./docs/20_qsa/qsa_originality.md)
-   [`docs/20_qsa/qsa_comparisons.md`](./docs/20_qsa/qsa_comparisons.md)
-   [`docs/40_implementations/zld/research_qsa-zd_originality_comparison.md`](./docs/40_implementations/zld/research_qsa-zd_originality_comparison.md)

---

## Roadmap / 今後の展開

-   Expand core documentation and theoretical underpinnings for SUI, QSA, IPS, and ZLD.
    （SUI、QSA、IPS、ZLD双方のコアドキュメントと理論的基盤の拡充。）
-   Provide diverse practical examples and case studies in the [`examples/`](./examples/) and [`docs/50_case-studies/`](./docs/50_case-studies/) directories.
    （[`examples/`](./examples/) および [`docs/50_case-studies/`](./docs/50_case-studies/) ディレクトリにおける多様な実用例とケーススタディの提供。）
-   Explore applications in LLM reasoning, autonomous agents, collaborative knowledge creation, and education.
    （LLM推論、自律エージェント、協調的知識創造、教育への応用探索。）
-   Develop prototype tools and interfaces embodying the SUI paradigm and QSA protocol.
    （SUIパラダイムとQSAプロトコルを具現化するプロトタイプツールやインターフェースの開発。）

---

## License / ライセンス

MIT License. See [`LICENSE`](./LICENSE) file.
（MITライセンス。[`LICENSE`](./LICENSE) ファイル参照。）

---
## Contributing / 貢献

Please refer to the [`CONTRIBUTING.md`](./CONTRIBUTING.md) file for guidelines on documentation, QSA loop recording, and general contributions.
（ドキュメント作成、QSAループ記録、および一般的な貢献に関するガイドラインについては、[`CONTRIBUTING.md`](./CONTRIBUTING.md) ファイルを参照してください。）
