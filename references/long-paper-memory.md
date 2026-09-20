# Long-paper and memory protocol

Use this protocol when the paper or resulting note would impose high navigation or recall cost. Common signals include a long or appendix-heavy PDF, more than roughly eight substantive themes, more than roughly twelve central concepts, dense cross-references, or a note that cannot be re-entered quickly. These are heuristics, not mandatory thresholds; activate the mode when it improves use.

The objective is not merely to shorten the note. Preserve the evidence while giving readers several entry depths and reliable ways to recover forgotten context.

## 1. Build a reading map first

Before drafting prose, map the paper:

| Section/range | Function in the argument | Reading depth | Why | Output destination |
|---|---|---|---|---|
| … | framing/method/evidence/appendix | deep/targeted/skimmed/unreadable | … | main note/supplement/omitted |

Record skipped, skimmed, inaccessible, or OCR-uncertain regions. Do not imply full coverage when reading was selective.

## 2. Provide four entry depths

The main note starts with four clearly distinguishable layers:

1. **L0 — 30-second orientation**: one-sentence takeaway, paper type, why it matters, largest conclusion-changing risk.
2. **L1 — 3-to-5-minute overview**: 200–300 words covering problem/scope, approach or synthesis method, strongest evidence, conclusion, and boundary.
3. **L2 — 10-to-20-minute conceptual spine**: the minimum concepts and argument chain needed to understand the paper.
4. **L3 — evidence on demand**: detailed methods, equations, tables, study clusters, related papers, and audits.

L0–L2 must be understandable without opening supplements. Each compression level is derived from the same evidence and must not introduce a stronger claim than the detailed note.

## 3. Add goal-based reading paths

Near the top, link to the sections needed for common goals. Adapt the paths to actual content:

- **Quick understanding**: L0 → key concepts → strongest result/synthesis → largest limitation.
- **Reproduction or implementation**: method → data/materials → evaluation → reproduction card.
- **Literature-review writing**: scope → concept boundaries → synthesis matrix → disputes/gaps → related literature.
- **Presentation or teaching**: L0 → conceptual spine/diagram → three evidence points → two caveats.

Do not list a path to an empty or inapplicable section.

## 4. Use memory anchors sparingly

Start a substantial analytical section with a compact anchor when readers would otherwise need to reconstruct context:

```markdown
> **本节记忆锚点**
> - 本节回答：
> - 一句话答案：
> - 前置概念：
> - 与上一节的关系：
> - 最重要证据：
> - 最容易混淆或忘记：
```

Do not repeat the block mechanically for short sections. End a long section with one or two retrieval questions or a short bridge to the next section.

## 5. Organize concepts as clusters

For a concept-heavy paper, group concepts by relationship rather than presenting one long glossary:

- parent/subtype;
- component/system;
- cause/effect;
- competing schools or methods;
- historical replacement;
- commonly confused terms.

Each cluster begins with a short relationship statement. Concept entries still follow the concept-explanation protocol and retain provenance.

## 6. Create a retrieval pack

At the end, write 5–8 high-value questions across three levels:

- **Recognition**: identify the concept, result, or distinction.
- **Explanation**: explain why a relation, method, or conclusion holds.
- **Transfer**: apply it to a new case or state when it would fail.

Answers must be recoverable through links or location anchors in the note. Avoid trivia and questions whose answer is only a name or date.

Add a compact recovery block:

```markdown
## 遗忘后从这里恢复

- 先恢复的 3 个概念：
- 最关键的 2 条证据：
- 最重要的 1 个边界：
- 主线图或论证链：
- 重新进入正文：
```

This is a reconstruction aid, not another summary of every section.

## 7. Split only when navigation improves

Default to one Markdown note. Use a small bundle when keeping everything in one file would bury L0–L2 or make evidence hard to retrieve:

```text
[first-author-year]--[short-title]/
|-- index.md
|-- concepts.md
|-- evidence.md
|-- related-literature.md
`-- figures/
```

Rules:

- `index.md` is the only required entry point and contains L0–L2, key conclusions, boundaries, and links.
- Create only supplements that contain substantial material; never create empty placeholders.
- Keep one source of truth for each claim. The main note summarizes and links instead of duplicating detailed tables.
- Use stable relative links and meaningful headings.
- A bundle is still one deliverable. Do not split mechanically by the paper's section numbers.
- If the user requested a single file, keep one file and place low-priority detail in appendices or portable `<details>` blocks.

## 8. Paper-type checkpoints

For a research paper, each method/result module should make recoverable: purpose, inputs, mechanism, evidence, and failure boundary.

For a review paper, each theme should make recoverable:

- the question the theme addresses;
- its dominant routes or theories;
- where evidence agrees;
- whether disagreements arise from definitions, data, methods, settings, or time;
- the most defensible current conclusion.

## 9. Optional review state

Only when useful to the user's workflow, add:

```yaml
memory_status: "new | reviewed | stable | needs-review"
last_reviewed: null
next_review: null
```

If the user has no review schedule, suggest checkpoints after the initial read, after a short delay, and after a longer delay rather than claiming a universal optimal interval. Update status from actual recall performance, not merely from rereading.

## 10. Compression quality check

Before delivery, verify:

- a reader can identify the paper and its value from L0;
- L1 states evidence and boundary, not only topic;
- L2 shows relations among concepts and claims;
- details remain traceable from summaries;
- memory anchors reduce context reconstruction rather than repeat headings;
- the recovery block points back into the note;
- splitting, if used, reduces navigation cost and leaves no orphan supplement.
