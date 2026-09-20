# Visual-note specification

## Selection and output

Only draw a diagram when it reveals a relationship, process, hierarchy, trade-off, or time pattern more clearly than prose/table. A full note normally uses 2–5 visuals; a short or metadata-only note may use none. Every visual has a purpose, source anchors (`derived from p. …`), an extracted-fact versus analyst-synthesis boundary, and Markdown alt text.

Use `diagram-design` with default **minimal-light** `assets/template.html`, self-contained HTML, and `doc-wide` size for Markdown notes. Save in the note's sibling `figures/` directory. Apply its style gate, chosen type/semantic-pattern reference, accessibility contract, complexity budget and self-check. Do not substitute Mermaid, screenshots or ASCII. Do not export PNG/SVG unless requested.

## Visual plan

| Paper | Priority | Visual | Diagram-design type | Caution |
|---|---:|---|---|---|
| Research | 1 | Problem→method→evaluation chain | Process/Data flow | Label inferred transitions. |
| Research | 2 | Architecture/components | Architecture/Layer stack/Tree | Only when interfaces are reported. |
| Research | 3 | Experiment or data flow | Flowchart/Timeline/Process | Do not imply unreported controls. |
| Research | 4 | Results comparison | Bar/Line/Scatter/Radar | Replot only unambiguous values. |
| Research | 5 | Limitations/failure modes | Fishbone/Quadrant/Layer stack | Separate author and analyst risks. |
| Review | 1 | Domain knowledge map | Tree/Nested/Layer stack | Avoid giant citation networks. |
| Review | 2 | Field evolution | Timeline | Mark contested groupings. |
| Review | 3 | Evidence selection | Flowchart | Never invent PRISMA counts. |
| Review | 4 | Method/application comparison | Quadrant/Radar/Bar | Use table when axes are weak. |
| Review | 5 | Gaps and roadmap | Process/Gantt/Fishbone | Label note synthesis explicitly. |

```markdown
### 图 1. 方法与证据链
![从问题定义、输入数据、核心机制到评估结果的流程图。](figures/short-title--method-flow.html)

*图 1：基于论文 §3–§5 整理；箭头和分组是分析性概括，不代表作者原图。*
```

For a numeric chart state metric, directionality, unit, dataset/task, and source table/figure. Never encode uncertain values as precise bars.

