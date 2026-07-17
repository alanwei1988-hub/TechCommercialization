# Deliverable Schema 2.0

Use one structured analysis source to create two format-specific deliverables. Preserve common IDs and evidence, but do not reuse the same visual structure across formats.

## Contents

1. Default package
2. Shared-source contract
3. 商业化分析 PPT contract
4. 论文列表 Excel sheet order
5. Workbook usability rules
6. Cross-file consistency
7. Optional formats
8. Package completion gate

## Default package

Deliver exactly these two files unless the user requests another scope:

1. **商业化分析 PPT**
   - Chinese filename: `<institution>_<scholar>_商业化分析.pptx`
   - Role: recommendation, self-reading, live presentation, and scholar discussion.
2. **论文列表 Excel**
   - Chinese filename: `<institution>_<scholar>_论文列表.xlsx`
   - Role: searchable publication index, evidence traceability, and later deep dives.

For reports in another language, localize filenames and visible labels while preserving these roles.

Do not generate Word, HTML, PDF, or Markdown by default. Create them only when explicitly requested.

## Shared-source contract

Maintain stable identifiers across files:

- Papers: `P01`, `P02`, and so on.
- Market and company sources: `S01`, `S02`, and so on.
- Commercial claims: `C01`, `C02`, and so on when a claim-level map is useful.
- Opportunities: one stable short label per opportunity, with zero or one marked `Lead Wedge`. When no option is responsibly supportable, record `No Responsible Lead Wedge Yet` and the evidence required to revisit the decision.

Use one structured source for identity, papers, directions, opportunities, scores, market evidence, interview questions, and limits. Create separate PPT and Excel presentation models from that source. Never paste the workbook layout into slides.

## 商业化分析 PPT contract

Use a 16:9 management-consulting-style deck that an MBA-level generalist can understand without oral narration. The core deck supports a commercialization decision; detailed scholar-interview prompts belong in the appendix or speaker notes.

Required characteristics:

- Start from the standard 21-slide skeleton in `presentation-report-guide.md`. A concise case may use 18-20 core slides; a regulated, hardware, clinical, or manufacturing case may require more than 22. Readability and decision completeness override the range.
- Give each slide one management question and one primary claim.
- Use declarative action titles rather than topic labels. Reading only the titles must reproduce the complete executive argument.
- Keep the cover neutral: show scholar, institution, scope, date, and decision question without stating the recommendation.
- Use slides 2-3 for a concise scholar whole picture: verified identity/title, field, active research years, research themes and evolution, representative work, and academic influence. Do not use a contents page or extended biography.
- By slide 5 at the latest, show which research themes deserve commercial attention and state the first commercialization recommendation—or explicitly state that no responsible first direction can yet be recommended and what evidence is missing.
- Present customer pain, buyer, current solution, and purchase logic before detailed methods, paper summaries, or technical architecture. A concise opening research map is the only exception.
- Keep the main deck commercial and decision-oriented; move detailed paper lists and source inventories to the Excel workbook or appendix.
- Show source IDs in a restrained footer or evidence note on every evidence-bearing slide.
- Use plain Chinese business labels in visible slides. Prefer `首选切入点`, `建议推进 / 保留观察 / 暂不投入`, `第一版可售产品`, and `足以叫停项目的风险` over unexplained English labels.
- Put at most two or three decision-changing questions on the final core slide. Put six to eight must-ask scholar questions and the full list in appendix slides or speaker notes.
- End on decisions, validation actions, or scholar questions, not a generic thank-you slide.
- Add or split slides whenever necessary to keep all decision-critical content complete, MBA-reader-friendly, and within the minimum font sizes. Do not combine independent narrative jobs into a dashboard merely to reduce page count.
- No visible PPT text may be shortened with `…`, `...`, text clamp, substring slicing, or hidden overflow. Long detail belongs on a new slide, in the appendix, or in speaker notes.
- No rendered line may begin with stranded punctuation, leave a one-character orphan, or split an English word or meaningful technical/commercial term. Native text bounds must remain inside their usable shapes.
- A per-slide QA log is part of the internal completion evidence even though it is not a default user-facing deliverable. It must include title-story and MBA-reader checks in addition to layout checks.
- Academic-influence metrics must use a named database, retrieval date, unit, and like-for-like comparison basis. Citation counts, h-index, publication volume, and honors must not be presented as customer-demand evidence.

Follow the required story arc and slide-level rules in `presentation-report-guide.md`.

## 论文列表 Excel sheet order

Use no more than four default sheets:

1. `Paper List`
2. `Selected Evidence`
3. `Directions & Timeline`
4. `Sources & Limits`

Do not include the former `Commercialization Snapshot`, `Product Blueprint`, `Market Solutions`, `Startup Design`, `Next Three Steps`, `Commercialization`, `Benchmarks`, or `Interview Questions` sheets by default. Their decision content belongs in the 商业化分析 PPT. Add a specialized sheet only when the user explicitly requests it or when the domain requires a structured record that cannot fit one of the four sheets.

### Paper List

Purpose: provide a complete, filterable, one-row-per-paper evidence index.

Required columns:

- Paper #
- Year
- Title
- Venue
- Type
- Authors
- Research Direction
- Technical Note
- Plain-Language Explanation
- Application Scenario
- Commercial Relevance
- Evidence Confidence
- Known Limit
- DOI / arXiv / URL
- Local PDF Path
- Download Status
- Used in PPT Slides

Rules:

- Assign every included work a stable paper number.
- Keep `Year` numeric and source URLs as usable hyperlinks/plain-text URLs.
- Make `Technical Note` compact; reserve deeper analysis for `Selected Evidence`.
- Explain what the result is, why it matters, and where it might be used without assuming domain expertise.
- Separate proven findings from inferred applications.
- Use `High / Medium / Low` or another documented vocabulary consistently for relevance and confidence.
- Record rejected near-duplicates or uncertain authorship in `Sources & Limits`, not as silently deleted rows.

### Selected Evidence

Purpose: connect PPT claims and opportunity judgments to the strongest supporting or challenging evidence.

Required columns:

- Claim ID
- PPT Slide
- Claim or Decision
- Evidence Type
- Paper # / Source #
- Evidence Summary
- Supports / Challenges / Limits
- Confidence
- Known Limit
- Next Validation

Allowed evidence types:

- `Technical Evidence`
- `Market Evidence`
- `Inference`
- `Interview Needed`

Rules:

- Include every major lead-wedge claim and each killer risk.
- Include contradictory evidence rather than building only a confirmation case.
- Use exact PPT slide numbers only after the final deck order is fixed.

### Directions & Timeline

Purpose: show how the publication corpus forms research capabilities and how those capabilities evolved.

Recommended columns:

- Direction
- Buyer-Readable Capability
- Active Years
- Paper Count
- Representative Papers
- Academic Influence Signal and Source Date
- First Key Node
- Strongest Evidence
- Recent Pivot
- Commercial Meaning
- Commercial Priority
- Main Limit

### Sources & Limits

Purpose: preserve auditability for scholar identity/title, bibliometric indicators, papers, market facts, companies, policies, procurement, regulation, and unresolved assumptions.

Assign an `Sxx` source record to any non-paper technical asset used as evidence, including prototypes, code repositories, datasets, patents, instruments, protocols, or deployment records.

Required columns:

- Source #
- Source Type
- Title / Entity
- URL / DOI / Local Path
- Date Accessed
- Claim Supported
- Used in PPT Slides
- Confidence
- Known Limit

## Workbook usability rules

- Freeze the header row and key identifier columns where helpful.
- Apply filters to every evidence table.
- Use readable widths, wrapping, and row heights; do not make every column equally wide.
- Use color to communicate direction, relevance, confidence, or status, but repeat the meaning in text.
- Keep gridlines hidden when explicit table styling defines the structure.
- Avoid decorative charts. Add a compact timeline or direction summary only when it improves evidence navigation.
- Keep the workbook machine-readable: one field type per column, one paper per row, no merged cells in data tables.
- Render and inspect all four sheets at normal zoom before export.
- Do not visually truncate cell values or replace them with ellipsis. Keep the stored value complete and use sufficient column width, wrapping, row height, or a dedicated detail field so the intended text is readable in the rendered sheet.
- `Plain-Language Explanation` must be understandable without specialist training; define necessary acronyms or technical terms in everyday language.

## Cross-file consistency

Before delivery, verify:

- Every paper number referenced in the PPT exists in `Paper List`.
- Every source number shown in a PPT footer exists in `Sources & Limits`.
- Every opening scholar-profile fact and influence indicator maps to an official profile or named scholarly database in `Sources & Limits`, with retrieval date and measurement unit.
- Every core PPT claim appears in `Selected Evidence`.
- Claim-to-slide coverage is semantic, not limited to slides that visibly print the `Cxx` ID: list every core slide where the claim is materially asserted.
- Opportunity names, judgments, scores, and confidence labels match across structured source and PPT.
- Final slide numbers populate `Used in PPT Slides` after the deck order is locked.
- File names use `商业化分析` for the PPT and `论文列表` for the Excel workbook.
- Scholar title, research duration, paper counts, citation indicators, and representative-work labels match the structured source and use one declared database per comparison.

## Optional formats

When the user explicitly requests Word or HTML:

- Treat the requested format as a separate editorial product, not a conversion of Excel tables.
- Preserve the same decision-first story and evidence IDs.
- For Word, read `word-report-finalization.md` and use the documents skill.
- For HTML, use narrative sections and progressive disclosure; keep wide tables limited to the paper browser.

## Package completion gate

Do not deliver until:

- The PPT passes full-slide render review and overflow/overlap checks.
- The workbook passes key-range inspection, formula-error scanning, and full-sheet visual review.
- An MBA-level reader can identify within five minutes what to pursue, who pays, what is sold, why the customer switches, why this team can win, what could stop the case, and what happens in the next 90 days.
- The opening establishes who the scholar is, their verified title and field, how long the research program has developed, its major themes, and its academic influence before commercial prioritization.
- Reading only the core-slide titles yields a coherent progression from scholar whole picture to research priorities, commercial recommendation, customer case, execution, and next decision.
- The customer problem and purchase logic appear before detailed research methods or paper summaries; only the concise opening whole-picture map may precede them.
- The scholar-discussion slide contains concrete questions that can change the recommendation.
- All claims are traceable and unsupported facts are labeled `需要验证`.
- Every slide and every rendered worksheet passes the zero-truncation check; no layout-created `…` / `...`, clipped character, or hidden overflow remains.
- Every slide passes the rendered-line integrity check: no stranded line-start punctuation, one-character orphan, split term/word, native text-bound escape, or actual-bound collision.
- The saved per-slide QA record shows `PASS` for ordinary-reader readability, minimum font, truncation, overflow/overlap, and citation legibility on every slide.
