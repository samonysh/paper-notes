# Concept explanation protocol

Use this protocol for concepts whose meaning materially affects comprehension, comparison, or reuse of the paper. A review paper normally needs a compact concept dictionary because definitions often determine its scope, taxonomy, and apparent disagreements.

## 1. Select concepts

Create a candidate list from the title/abstract, research questions, keywords, section headings, taxonomy labels, repeated contrasts, formal definitions, and unfamiliar acronyms. Retain a concept when at least one condition holds:

- it defines what the paper includes or excludes;
- it is an axis of the paper's taxonomy or synthesis;
- it is field-specific, overloaded across disciplines, recently coined, or used inconsistently;
- misunderstanding it would change the interpretation of a method, result, controversy, or limitation;
- the paper assumes it without an adequate definition.

Do not explain ordinary words or create an exhaustive glossary. Prefer roughly 5–12 core concepts for a substantial review and 3–8 for a research paper, adjusting to actual complexity.

## 2. Use the source ladder

Establish meaning in this order:

1. **Paper usage** — quote or paraphrase the paper's explicit definition and record a page/section anchor.
2. **Cited or originating source** — follow the paper's reference when the term is attributed, contested, or introduced elsewhere.
3. **Authoritative external source** — prefer standards bodies, professional societies, official documentation, scholarly encyclopedias, university materials, textbooks, or peer-reviewed review articles.
4. **LLM synthesis** — use model knowledge to explain the idea in simpler language or connect sources, clearly labelled `LLM 综合`; it is an explanatory aid, not an authority or citation.

Browse when a central concept is undefined, ambiguous, unfamiliar, time-sensitive, or disputed. Do not browse merely to decorate an adequate paper definition. Never use a search-result snippet as the cited source, and do not use an unsourced aggregator or Wikipedia as the sole authority for a consequential definition.

## 3. Write a concept entry

Each important concept should answer:

- **一句话通俗解释**：what it means without relying on the term itself;
- **技术含义**：necessary conditions, mechanism, variables, or formal meaning;
- **本文中的角色**：why this paper needs the concept;
- **边界与易混概念**：what it is not, nearby terms, and where usage differs;
- **依据**：`论文定义` / `外部来源` / `LLM 综合`, with paper location or external citation;
- **可信度**：high/medium/low when the explanation requires inference or sources disagree.

Use prose for the concepts that form the paper's conceptual spine. A table may compact the remaining entries, but must not reduce a disputed concept to a one-line dictionary gloss.

```markdown
### [概念名]（[English term / acronym]）

**通俗解释：** …

**技术含义与本文角色：** …

**边界：** 与 `[相邻概念]` 的区别是 …；本文采用的是 … 口径。

**依据：** [论文定义，p. X, §Y / 外部来源：作者或机构，标题，URL/DOI，访问日期 / LLM 综合]
**可信度：** 高/中/低；[必要说明]
```

## 4. Resolve conflicts

When definitions conflict, do not silently choose one. State:

1. the paper's operational meaning;
2. the alternative meaning and its source;
3. whether the disagreement is terminological, methodological, or substantive;
4. how it changes the review's grouping, comparison, or conclusion.

For a review paper, distinguish **author-proposed taxonomy**, **field-established taxonomy**, and **analyst reconstruction**. Label merged categories and inferred relationships explicitly.

## 5. Keep provenance separate

Paper claims remain anchored to the paper. External concept sources belong in a separate list:

| 概念 | 外部来源 | 用途 | 访问日期 |
|---|---|---|---|

An external source may clarify terminology; it does not become evidence for the reviewed paper's empirical or synthesis conclusions. If no suitable source is available, say so and label the explanation `LLM 综合 / 待核验`.

## 6. Add retrieval cues

Turn the conceptual spine into 3–7 non-trivial questions that can be answered from the note, for example:

- Why does the paper distinguish A from B, and which conclusions depend on that boundary?
- Under what conditions does method C cease to fit the paper's definition of D?
- Which disagreement disappears when two sources use the same operational definition?

Prefer questions that test relationships, boundaries, and use cases over simple term recall.
