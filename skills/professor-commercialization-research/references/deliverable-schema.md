# Deliverable Schema

Prefer a structured workbook for iterative research. Use Word or readable HTML when the user wants a polished narrative artifact. Final user-facing deliverables must be Excel, Word, or readable HTML unless the user explicitly requests another format; Markdown is acceptable only as an internal note or source draft.

## Recommended workbook sheets

### Overview

Purpose: give the user a one-screen orientation.

Columns or sections:

- Professor/lab identity
- Time window
- Total included works
- Downloaded PDFs
- Main research directions
- Most commercially relevant directions
- Key caveats

### Paper Browser

Purpose: enable paper-by-paper filtering and review.

Recommended columns:

- Paper #
- Year
- Title
- Venue
- Type
- Authors
- Research Direction
- Technical Keywords
- Analysis Summary
- Plain-Language Explanation and Application Scenarios
- Commercial Relevance
- Evidence Confidence
- DOI/arXiv/URL
- Local PDF Path
- Download Status

The `Plain-Language Explanation and Application Scenarios` column is mandatory. It must explain, for a non-specialist reader, what the result is, why it matters, and where it might be used.

### Directions

Purpose: summarize research clusters.

Recommended columns:

- Direction
- Paper Count
- Representative Papers
- Core Capability
- Main Evidence
- Industrial Pain Point
- Productization Potential
- Key Limits

### Timeline

Purpose: show research evolution.

Recommended columns:

- Year
- Representative Papers
- Direction
- Technical Milestone
- Commercial Meaning
- Notes

### Deep Dives

Purpose: test selected commercialization hypotheses.

Recommended columns:

- Paper #
- User Hypothesis
- Evidence Found
- Accuracy Judgment
- Better Product Framing
- Missing Work
- Suggested Next Validation

### Commercialization

Purpose: translate research into possible company strategy.

Recommended columns:

- Opportunity
- Target Customer
- Pain Point
- Research Basis
- Product Form
- Buy-vs-Build Risk
- Competitive Pressure
- Go-to-Market Wedge
- Readiness
- Recommendation

### Commercial Benchmarks

Purpose: compare domestic and international commercial companies, adjacent platform products, open-source substitutes, and true white spaces. The sheet may be named `Benchmarks` for compatibility, but the title/header should make clear it means "国内外商业化公司对标或空白".

Recommended columns:

- Direction
- Foreign Commercial Companies
- Domestic Commercial Companies
- Adjacent Platforms / Open Source Substitutes
- What They Sell or Provide
- Benchmark Directness (direct product, adjacent product, platform feature, open source, or blank)
- Differentiation Gap
- White Space / Blank Reason
- Source Links

### Interview Questions

Purpose: give a technical manager a targeted question list for interviewing the scholar after the research and commercialization analysis.

Default orientation: the list should help a non-specialist technical manager conduct business analysis, demand/resource diagnosis, technology maturity judgment, company design, operating-governance review, and next-step consulting design. Technical questions should appear mainly as plain-language follow-ups or evidence prompts.

Recommended columns:

- Section
- Priority
- Main Question
- Plain-language Follow-up
- Commercialization Purpose
- Evidence From Analysis
- Expected Signal / Decision Use
- Related Paper # or Direction
- Notes During Interview

The questions must be specific to the scholar's actual research directions and commercialization evidence. Avoid generic questionnaires that could apply to any professor.

## HTML report structure

- Executive summary
- Research directions
- Timeline
- Paper table or browser
- Selected deep dives
- Commercialization options
- Domestic/international commercial-company benchmarks or white spaces
- Targeted scholar interview questions
- Sources and limits

HTML must be readable as a standalone report, with tables, anchors, filters, or section navigation when the corpus is large.

## Word report structure

- Executive summary
- Research trajectory and key nodes
- Plain-language explanation of major results
- Selected deep dives, if the user chose any
- Commercialization judgment
- Domestic/international commercial-company benchmarks or white spaces and build-vs-buy analysis
- Targeted scholar interview question list
- Sources and limits

## Style rules

- Keep technical summaries compact and sourced.
- Make plain-language summaries useful to a non-specialist investor or operator.
- Label inference clearly.
- Avoid "promising" language unless the evidence supports product readiness.
- Prefer "possible wedge" or "requires validation" for early-stage ideas.
