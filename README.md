# paper-notes

A Codex skill for turning an academic paper PDF or URL into an evidence-traceable Chinese Markdown note.

## What it adds

- paper claims, evidence, external context, and analyst judgments are explicitly separated;
- research papers and review papers use different note structures;
- important concepts receive plain-language and technical explanations with provenance labels;
- a bounded set of cited or related papers is retrieved and selectively read;
- review notes synthesize by theme and evidence relationship instead of listing papers one by one;
- diagrams are created only when they improve understanding.

## Concept provenance

Every enriched concept is labelled as one or more of:

- **论文定义** — the focal paper's own definition, with location;
- **外部来源** — a cited/original or authoritative source, with URL/identifier and access date;
- **LLM 综合** — a plain-language synthesis that is not treated as scholarly evidence.

External explanations and related-paper findings never enter the focal paper's evidence ledger.

## Related-paper retrieval

The skill routes retrieval by purpose:

- `papers-cool-search` for focused, current AI/CS discovery;
- `paper-search` or authoritative indexes for exact citations, broader disciplines, and fuller coverage;
- canonical publisher/repository pages for version and passage verification.

A note normally deepens only 3–8 related papers. Keyword similarity is not described as a citation relationship.

## Structure

```text
paper-notes/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── acquisition-and-reading.md
    ├── concept-explanation-protocol.md
    ├── related-literature-protocol.md
    ├── research-paper-template.md
    ├── review-paper-template.md
    └── visual-note-spec.md
```

## Design references

The templates adapt several established note and review practices:

- [Cornell Note-Taking System](https://lsc.cornell.edu/notes.html): concise summaries, retrieval cues, questions, reflection, and review.
- [University of Sheffield literature review guidance](https://www.sheffield.ac.uk/study-skills/writing/critical/literature-review): literature and synthesis matrices organized around themes and relationships among sources.
- [George Mason University Writing Center on literature-review organization](https://writingcenter.gmu.edu/writing-resources/research-based-writing/organizing-literature-reviews-the-basics): synthesis rather than a chain of source summaries.
- [Purdue OWL literature review guidance](https://owl.purdue.edu/owl/research_and_citation/conducting_research/writing_a_literature_review.html): summarize, synthesize, analyze, interpret, and critically evaluate.
- [PRISMA 2020](https://www.prisma-statement.org/prisma-2020): reporting checks for systematic reviews, used here as reporting guidance rather than a quality score.
- [Zettelkasten literature/permanent note workflow](https://zettelkasten.de/posts/concepts-sohnke-ahrens-explained/): self-contained, reusable notes written in the reader's own words.

These sources informed the structure; the repository does not reproduce their templates verbatim.

## Use

Invoke the skill with a local PDF or paper URL:

```text
Use $paper-notes to read this paper and create a Chinese Markdown note with evidence locations, concept explanations, and related-paper verification.
```

The skill is designed for analysis and note construction, not full-paper translation.
