# Acquisition and reading protocol

## Source record

Record the requested input, canonical PDF/landing URL, access date, arXiv/published version, title/authors/year/venue/DOI or ID, access level, and extraction quality (`native text`, `mixed`, `OCR`, or `unreadable regions`). Never silently substitute versions.

## URL routing

| Input | Procedure |
|---|---|
| Local `.pdf` | Verify the file; extract metadata/text; inspect page count and render difficult pages. |
| arXiv abstract, PDF, HTML, or export URL | Normalize ID and requested version; retrieve the official PDF endpoint; retain the requested version. Landing metadata supplements, not replaces, PDF. |
| DOI/publisher URL | Resolve landing page; use an authoritative open PDF or a supplied copy. Do not evade access controls. |
| Institutional repository | Verify title/authors/version against its metadata; retrieve the openly supplied PDF. |
| HTML full text | Read complete accessible content; cite section anchors when PDF pages do not exist. |

If content is inaccessible, state what was available and produce only a labelled metadata/abstract-level note.

## Evidence ledger

| Claim/field | Value or paraphrase | Evidence location | Evidence kind | Confidence | Caveat |
|---|---|---|---|---|---|
| Main problem | `…` | `p. 1, §1` | author statement | high | — |
| Result R1 | `…` | `p. 8, Table 3` | reported result | high | specific dataset |
| Limitation | `…` | `p. 10, §6` | author statement | medium | no external validation |
| Interpretation | `…` | `inference from R1/R2` | analyst inference | medium | needs replication |

Use two passes: map the argument from abstract, introduction, figures/tables, conclusion; then inspect methods, results, appendices, validity threats and evidence needed by the note. For empirical papers capture sample/data provenance, splits, baselines, metrics and uncertainty; for qualitative work capture setting, participants, collection, coding, reflexivity and transferability; for theoretical work capture notation, assumptions, theorem/claim numbers and proof dependencies.

Maintain a separate concept-source ledger when external material is used. Record concept, canonical source, source type, access date, the point clarified, and whether the resulting explanation is quoted, paraphrased, or LLM-synthesized. External context must not be presented as if it appeared in the paper.

## Related-paper ledger

When a cited or externally discovered paper is read, record its relationship to the focal paper, canonical identifier/URL, version read, access level, relevant passage location, extracted point, and selection rationale. Keep `本文引用` separate from `检索补充`, and never describe keyword-similar papers as citation-linked without citation evidence.
## Figure/table/equation rule

Read captions, axes/legends and nearby interpretation together. State what an exhibit supports and does not support. Recreate only a small transparent derived table/chart; otherwise cite its location. Flag unreadable scans, truncated appendices and OCR uncertainty.

## Quality pass

Every main claim needs a location; every number needs unit, baseline and condition; version is explicit; author claims, external context, and analyst critique are distinct; concept explanations show their basis; no conclusion exceeds the evidence.

