# Related literature protocol

Use this protocol when a paper mentions, cites, contrasts with, or depends on another paper and reading that work would materially improve the note. The goal is a bounded evidence expansion, not an exhaustive citation graph.

## 1. Decide what to follow

Prioritize related papers that serve at least one role:

1. **Concept origin** — introduces or defines a central term, taxonomy, dataset, benchmark, or method.
2. **Evidence dependency** — is the main support for a consequential claim that the current paper does not itself establish.
3. **Closest comparison** — supplies the baseline, competing theory, or directly contrasted result needed to understand novelty.
4. **Synthesis anchor** — is repeatedly used by a review paper to define a theme, period, school, or consensus.
5. **Conflict or update** — challenges the paper's synthesis or materially updates it.

Normally deepen 3–8 papers. Raise the cap only when the user requests a broader literature map. Do not fetch every bibliography entry.

## 2. Route the search

- **Exact cited work**: search the title, DOI, arXiv ID, or other identifier. Prefer the canonical publisher/repository record and verify title, authors, year, and version.
- **Current AI/CS neighbors**: use the installed `papers-cool-search` skill when available. Use topic/category/venue search for discovery or one-hop REL for a seed paper. REL is a card-keyword search, not a citation graph; label it accordingly and never recurse automatically.
- **Broad or cross-disciplinary search**: use the installed `paper-search` skill or authoritative scholarly indexes such as Crossref, OpenAlex, Semantic Scholar, PubMed, or discipline-specific repositories.
- **Citing/follow-up work**: use a source that exposes citation relations when available. Do not infer “cites” or “is cited by” from keyword similarity.
- **Unavailable tools**: use web search with exact titles/identifiers and prefer canonical scholarly landing pages. Never invent bibliographic metadata.

Use search sources as discovery layers. For precise claims, versions, publication status, or passages, follow the canonical source and read the paper itself when lawful full text is available.

## 3. Verify and read selectively

For every retained paper:

- deduplicate preprint and venue versions; preserve both links when useful and identify the version read;
- record why it was selected and its relation to the focal paper;
- read the abstract plus the relevant definition, method, result, or discussion passage;
- capture a page/section/table/figure anchor when full text is available;
- distinguish abstract-only evidence from full-text verification;
- do not bypass paywalls, login walls, robots restrictions, or download controls.

If only metadata or an abstract is available, label the entry `metadata/abstract only` and do not make passage-level claims.

## 4. Integrate without contaminating provenance

Add external papers in a separate section or clearly labelled callout. Never make their findings look like evidence reported by the focal paper.

| 关联论文 | 与本文关系 | 提取内容 | 对理解本文的影响 | 阅读范围与定位 | 来源 |
|---|---|---|---|---|---|

Use these labels where useful:

- **本文引用** — explicitly present in the focal paper's references;
- **检索补充** — found externally and not known to be cited by the focal paper;
- **后续工作** — published later;
- **相反证据** — challenges a claim or synthesis;
- **概念来源** — clarifies a definition or origin.

After the table, write a short synthesis: what the external reading confirms, revises, or leaves unresolved. Do not treat citation count, popularity, recommendation rank, or an AI-generated summary as scholarly evidence.

## 5. Record retrieval provenance

For each search session record:

- route/tool and query or seed;
- search date;
- selection rule and stopping rule;
- canonical source URL/DOI/arXiv ID;
- access level (`full text`, `abstract only`, or `metadata only`).

For papers.cool, retain both the papers.cool discovery URL and the canonical source URL. Distinguish arXiv preprints from peer-reviewed venue papers and state that papers.cool coverage is curated rather than exhaustive.
