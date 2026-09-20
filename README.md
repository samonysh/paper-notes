# paper-notes

A Codex skill for turning an academic paper PDF or URL into an evidence-traceable Chinese Markdown note.

## What it adds

- paper claims, evidence, external context, and analyst judgments are explicitly separated;
- research papers and review papers use different note structures;
- long papers use layered entry depths, reading paths, memory anchors, and a recovery pack;
- important concepts receive plain-language and technical explanations with provenance labels;
- a bounded set of cited or related papers is retrieved and selectively read;
- review notes synthesize by theme and evidence relationship instead of listing papers one by one;
- diagrams are created only when they improve understanding.

## Long-paper mode

When length or conceptual density makes a paper hard to re-enter, the skill adds:

- L0–L3 reading depths, from a 30-second orientation to evidence on demand;
- goal-based reading paths for quick understanding, reproduction, review writing, or presentation;
- selective memory anchors and concept clusters;
- recognition, explanation, and transfer questions;
- an “遗忘后从这里恢复” reconstruction block;
- an optional `index.md` plus small supplements bundle when one file would bury the core argument.

Page count is only a heuristic. The mode activates when it lowers navigation and recall cost without hiding evidence.
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
    ├── long-paper-memory.md
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
Use $paper-notes to read this paper and create a Chinese Markdown note with layered reading paths, evidence locations, concept explanations, memory recovery, and related-paper verification.
```

The skill is designed for analysis and note construction, not full-paper translation.
