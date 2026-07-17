---
name: professor-commercialization-research
description: Build a decision-first, evidence-backed commercialization analysis from a professor, researcher, PI, lab, or academic team name. Use when Codex needs to disambiguate an academic identity, build and clean a publication corpus, translate research into customer value, select and score one commercialization entry point, design products and commercialization routes, scan current solutions and benchmarks, prepare scholar interview questions, or deliver a scholar-shareable, management-readable 商业化分析 PPT plus a traceable 论文列表 Excel. Also use when the user says "技术商业化分析skill", "技术商业化分析", or asks for a technology commercialization analysis skill. If invoked without a target institution and scholar, first ask which institution/lab and scholar the user wants to study.
---

# Technology Commercialization Analysis 2.1 — Scholar-Shareable Consulting Edition

## Objective

Turn a professor or lab name into a management decision, not an academic review.

Use an MBA-level generalist as the internal comprehension benchmark. Unless the user specifies an internal-only memo or another recipient, assume the finished deck may be forwarded unchanged to the named scholar. Never print the reader persona or the production logic in the deliverable.

Use six operating principles:

1. **Orient briefly, answer early**: use two concise pages to show who the scholar is and how the research program fits together; identify commercial priorities and the recommendation by slide 5.
2. **Business question first after orientation**: organize the remaining core deck around customer pain, purchase logic, product, advantage, economics, execution, and risk—not around paper clusters or methods.
3. **One governing thought**: every slide title states one conclusion; the body proves it; the final line explains the decision implication.
4. **Plain language by default**: explain what the technology lets a customer do, save, earn, avoid, or decide. Put method names and paper detail in evidence notes or the appendix.
5. **Evidence without false certainty**: separate technical proof, market proof, inference, and facts that still require interviews. Score attractiveness separately from confidence.
6. **External-ready by default**: use formal, respectful, collaborative language; evaluate the readiness and evidence of a commercialization direction, not the academic worth of the scholar or the research.

## Default Delivery Contract

Unless the user explicitly requests another format, deliver exactly two user-facing files:

1. **商业化分析 PPT**: `<institution>_<scholar>_商业化分析.pptx`
2. **论文列表 Excel**: `<institution>_<scholar>_论文列表.xlsx`

Treat the PPT as the executive decision and scholar-conversation layer. Treat the Excel workbook as the searchable evidence layer. Build both from one structured source, but use different presentation models. Never convert workbook tables wholesale into slides.

Generate Word, HTML, PDF, or another narrative format only when the user explicitly requests it. Do not generate Markdown as a default user-facing deliverable.

Use the presentations skill for the PPT and the spreadsheets skill for the Excel workbook. Follow each format skill's implementation and visual-QA requirements.

## Audience and Readability Contract

- Write for a commercially trained non-specialist. Treat `MBA-readable` as an internal readability test, never as visible audience copy. Unless another recipient is named, the deck must pass a direct-send test for the scholar.
- Use the scholar's verified formal title or name in the cover and formal headings. Evaluate evidence, transfer readiness, product gaps, and market uncertainty; do not judge whether the scholar or the research is academically "worthy".
- Keep the cover neutral and externally shareable: show the scholar, affiliation, analysis scope, evidence date, and an optional qualifier such as `基于公开资料整理｜供交流讨论`. Do not expose the recommendation, reader persona, production process, or buyer-validation jargon. Avoid cover phrases such as `面向 MBA 毕业生`, `先看清`, `哪些成果值得`, `进入付费验证`, or `机会全景` when the opportunity set is not established.
- Use the first two content slides after the cover to establish the scholar's whole picture: verified identity and title, field, years of research, research themes and evolution, representative work, and academic influence. Keep this orientation concise and visual rather than turning it into a biography or literature review.
- Explain every unfamiliar metric on first visible use. State what the source or database is, what the number literally means, and what it does not prove. For example, explain `Scopus 收录文献` as documents attributed to the author's database profile, and explain `h=32` as at least 32 works having at least 32 citations each; neither proves market demand or research quality by itself.
- By slide 5 at the latest, make visible which research themes deserve commercial attention and what first direction is recommended. The next slides must make the customer problem, buyer, first offer, largest uncertainty, and immediate next step understandable without explaining algorithms.
- On the opportunity-prioritization slide, every direction must answer four questions: `方向是什么`, `第一笔钱买什么`, `谁会买并用于什么决策`, and `当前判断与最大证据缺口`. Treat any score as relative validation priority, not market size, success probability, revenue, or proof that the opportunity already exists.
- Do not place a full publication inventory, method taxonomy, CV, honor list, or opportunity-scoring methodology in the opening. The scholar overview is context; it must lead directly to research prioritization and a commercial recommendation.
- On first visible use, explain every necessary technical term in everyday Chinese. Showing the full English name does not count as an explanation.
- Use visible Chinese business labels. Prefer `首选切入点`, `建议推进 / 保留观察 / 暂不投入`, `第一版可售产品`, and `会让项目停止的风险` over unexplained English labels.
- Readability overrides slide count. Start with the standard consulting story in `references/presentation-report-guide.md`, then split any dense slide. Never shrink, omit, or truncate decision-critical content to hit a page target.
- Visible text must never be shortened by automatic ellipsis, manual `…` / `...`, substring slicing, or hidden overflow. Rewrite, resize, or split the slide.
- A rendered slide fails if a line begins with stranded punctuation, leaves a single-character orphan, or splits an English word or meaningful Chinese term.
- When Microsoft PowerPoint is available, compare each text shape's native `TextFrame2.TextRange.BoundWidth/BoundHeight` with its usable bounds. Any positive native overflow or actual collision blocks delivery.

Read `references/consulting-language-guide.md` before drafting any visible PPT copy. It defines the scholar-shareable voice, MBA-level readability benchmark, unfamiliar-metric explanations, jargon conversions, forbidden filler, and page-level writing checks.

## Invocation

If the user invokes only the skill name or says "技术商业化分析" without naming a target, ask one short question:

> 你想研究哪个机构的哪位学者？如果已有关注时间范围、重点产业方向或需要回答的商业问题，也可以一起告诉我。

If the institution and scholar are already provided, start without additional intake questions unless identity is ambiguous.

If scope is unspecified, use the scholar's full verifiable career for identity, research duration, theme evolution, representative work, and academic-influence context. Use the last 10 years as the default detailed publication-analysis window, including relevant peer-reviewed papers and preprints/chapters, and use the user's language.

## Required Executive Answers

Distribute these answers across the core decision story after the opening whole picture; do not cram them onto slides 4-5. Slide 4 prioritizes research themes and slide 5 gives the recommendation or an explicit `当前无法负责任地推荐首选方向`; later slides prove and operationalize the judgment. Use the plain Chinese labels below in visible content; internal structured fields may retain stable English keys.

| Decision field | Visible reader-facing question |
| --- | --- |
| Lead Wedge | `最值得先验证的切入点是什么？` |
| Portfolio judgment | `哪些方向建议推进、观察或暂不投入？` |
| Customer | `谁在为什么问题付钱？谁使用、谁决策、谁出预算？` |
| Product thesis | `第一版到底卖什么，交付后改变哪个客户结果？` |
| Purchase logic | `客户为什么买，而不是继续手工做、自己开发或采购现有方案？` |
| Proof | `我们为什么这样判断？哪些是事实，哪些仍是推断？` |
| Economics | `首个试点如何报价、如何交付、能否重复销售？` |
| Route | `更适合成立公司、授权、联合开发，还是先做专业服务？` |
| Readiness | `离付费交付还缺什么：产品、数据、验证、团队、IP还是审批？` |
| Killer risks | `哪两三件事一旦不成立，就应停止投入？` |
| Action | `未来90天做哪几项低成本验证，什么结果决定继续或停止？` |

Show one primary recommendation, no more than two secondary options, a commercial-attractiveness judgment, and a separate confidence level. If evidence is too thin, state that no responsible recommendation can yet be made.

## Workflow

1. **Scope and identity**
   - Confirm affiliation, department, lab, name variants, coauthors, and official pages.
   - Cross-check scholarly indexes such as ORCID, DBLP, Semantic Scholar, OpenAlex, Crossref, and field-specific sources.
   - Record assumptions and ambiguity before analysis.
   - Build a dated scholar snapshot: verified position/title, field, first and latest relevant work, active research years, publication/citation indicators, representative works, and peer context when a like-for-like comparison is possible.
   - Use one named scholarly database and one retrieval date for each bibliometric comparison. Do not mix citation counts across sources or present unsupported percentiles.

2. **Corpus and evidence index**
   - Build a publication table with a stable paper number, title, year, venue, authors, DOI/arXiv/URL, source, type, and inclusion status.
   - Deduplicate by DOI, normalized title, and author/year.
   - Download only lawful open PDFs or author copies and record download status.
   - Save structured metadata early so the PPT and Excel can be regenerated.

3. **Research-to-value translation**
   - Cluster papers internally by recurring problem, method, workflow, and application domain.
   - Create a plain-language whole-picture map with three to five research themes, active periods, representative contributions, and visible evolution. Use it in the opening before commercial prioritization.
   - Translate each cluster into three layers: `研究证明了什么` → `可以形成什么能力` → `可能改善哪个客户结果`.
   - Name external-facing clusters by the customer job or outcome, not the algorithm.
   - Identify reusable code, data, patents, protocols, validation access, trust, and domain know-how that could create a commercial advantage.

4. **Hypothesis-led commercial triage**
   - Frame no more than three mutually distinct opportunities.
   - Scan pain, buyer clarity, current solutions, productability, market timing, adoption burden, economics, defensibility, and transfer readiness.
   - Score opportunities using `references/commercialization-framework.md`, but keep scoring detail out of the early core deck.
   - Select exactly one first entry point unless the evidence is too thin.
   - Record technical proof, market proof, inference, counterevidence, and interview-needed facts separately.

5. **Paper analysis by decision value**
   - Give every included paper a compact technical note, plain-language explanation, application scenario, commercial-relevance label, confidence, and known limit in Excel.
   - Deep-read representative, commercially important, contradictory, recent-pivot, or user-selected papers.
   - Test every product claim against what the paper actually proves; do not turn laboratory performance into a customer promise.

6. **Optional user checkpoint**
   - After the numbered paper list and preliminary triage exist, ask once whether the user wants particular results deep-dived.
   - Use: "请选择需要深入分析的成果序号；也可以补充你的商业假设。没有也没关系，我会继续完成商业化分析 PPT 和论文列表 Excel。"
   - Continue autonomously if the user does not select papers.

7. **Customer, offer, economics, and route**
   - Define the job, current workaround, economic consequence, purchase trigger, user, decision maker, budget owner, and procurement path.
   - Define the first sellable offer, customer workflow, must-have features, success measure, explicit exclusions, and productization gaps.
   - Compare manual work, self-build, incumbents, platforms, open source, consulting, outsourcing, and doing nothing.
   - State a paid-pilot and pricing hypothesis when evidence permits; otherwise write `需要验证`.
   - Compare startup, licensing, joint development, service, component, and standards/audit routes instead of assuming a startup.

8. **Execution, IP, and validation plan**
   - Define the minimum operating team, PI and student roles, external commercial and engineering needs, governance boundaries, IP ownership, and university-transfer issues.
   - Identify two or three thesis-killing uncertainties.
   - Produce concrete 30/60/90-day experiments with owner, target, output, success signal, failure signal, and decision changed.
   - After deep reading and customer, economics, IP, and execution analysis, refresh every opportunity score, confidence level, hard blocker, and recommendation. Do not carry the preliminary triage judgment forward unchanged.

9. **Scholar-conversation design**
   - Convert the highest-impact unknowns into questions a generalist consultant can ask naturally.
   - Put at most two or three questions that directly change the requested decision on the final core slide.
   - Put six to eight must-ask questions and the complete prioritized list in appendix slides or speaker notes, not in the default Excel workbook.

10. **Build and validate**
   - Draft the title-only story spine before laying out slides. The titles alone must move coherently from scholar whole picture to research priorities, recommendation, customer case, execution, and next decision.
   - Build the PPT before finalizing the workbook's slide mappings.
   - Build Excel with the exact paper and source IDs used in the PPT.
   - Verify counts, links, evidence labels, source freshness, filenames, and cross-file references.
   - Render and inspect every slide and every worksheet at full size.
   - Run native text-bound checks when PowerPoint is available.
   - For repeated-row comparisons, use equal row geometry, aligned column anchors, vertically centered text groups, and explicit line breaks where automatic wrapping would make rows visually inconsistent. In narrow metric panels, separate the value, unit, label, period, and method; do not rely on a mixed string such as `19+` remaining on one line.
   - Save a per-slide QA record with one row per slide: slide number, action title, title-only story check, scholar-context/metric-source check, direct-send check, unfamiliar-metric explanation check, MBA-reader check, minimum-font check, ellipsis/truncation check, overflow/overlap check, citation-legibility check, status, and fix made. Any failed check blocks delivery.

## Evidence Rules

- Label important claims as `Technical Evidence`, `Market Evidence`, `Inference`, or `Interview Needed` in the structured source. Localize visible slide labels into clear Chinese.
- Browse and cite current market, company, product, policy, procurement, competitor, and regulatory facts.
- Never turn a technical result into a customer claim without marking the inference.
- Write `需要验证：<具体事实>` instead of inventing pain magnitude, price, willingness to pay, IP status, team commitment, or market size.
- Use stable paper and source numbers across PPT, Excel, local PDFs, and notes.
- Keep method names out of core slide titles unless the method itself changes the commercial decision.
- Do not use a bibliometric term in an action title unless the title or the same slide also states its plain-language meaning. Show database, retrieval date, unit, literal interpretation, and limitation for publication counts, citation counts, h-index, journal metrics, and field-normalized ranks.
- Put source identifiers in a restrained footer; explain the evidence in reader-facing language in the body.

## Completion Gates

Complete the default package only when:

- The title-only story states one recommendation, the customer case, the offer, the right to win, the economics, the main risks, and the next decision without relying on spoken explanation.
- The opening gives an MBA-level reader an accurate whole picture of who the scholar is, what fields and themes they have worked on, for how long, and their academic influence before asking the reader to evaluate commercialization priorities.
- The deck passes the direct-send test: every visible string is appropriate if read by the named scholar without accompanying explanation; no visible line describes the reader persona, prompt, workflow, slide-production process, QA, model, tool, or script.
- Every academic-influence metric names its database, retrieval date, unit, and comparison basis. Citation volume, h-index, publication count, and awards are never treated as direct evidence of customer demand.
- Every unfamiliar metric can be paraphrased by a non-specialist after one reading; the slide explains what the number means and what it cannot establish.
- An MBA-level reader can identify within five minutes: what to pursue, who pays, what is sold, why the customer switches, why this team can win, what could kill the thesis, and what happens in the next 90 days.
- Research history and method detail support the recommendation rather than drive the core narrative.
- Every major commercial claim maps to a paper number, source number, explicit inference, or interview-needed fact.
- The Excel workbook starts with `Paper List`, uses one row per paper, supports filtering, and includes plain-language meaning and application scenarios.
- PPT paper and source references resolve in Excel without mismatch.
- Recommendation and confidence are visible, separate, and not overstated.
- Every core slide passes the page grammar: one action title, focused evidence, and a clear decision implication.
- Every core slide passes the MBA-reader test: the reader can state the conclusion, why it is true or uncertain, and what it changes after one reading.
- The opportunity-prioritization slide makes each direction's product or service form, first paid deliverable, buyer and decision, validation status, and largest evidence gap explicit; its repeated rows share a consistent visual center in the native PowerPoint render.
- No visible string ends in a layout-created `…` or `...`; no text is hidden, clipped, orphaned, or split across lines.
- A complete per-slide QA record exists and every slide is marked `PASS`; montage-only review is insufficient.
- Word and HTML are absent unless explicitly requested.

## References

- Read `references/workflow-checklist.md` when starting a new scholar/lab project.
- Read `references/commercialization-framework.md` before scoring opportunities or designing products, economics, teams, and commercialization routes.
- Read `references/presentation-report-guide.md` before planning or creating the 商业化分析 PPT.
- Read `references/consulting-language-guide.md` before drafting visible PPT titles or body copy.
- Read `references/deliverable-schema.md` before creating the PPT/Excel package.
- Read `references/interview-question-guide.md` before writing the scholar-discussion slide, appendix questions, or speaker notes.
- Read `references/word-report-finalization.md` only when the user explicitly requests a Word report.
