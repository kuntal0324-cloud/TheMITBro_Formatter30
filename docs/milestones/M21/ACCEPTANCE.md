# TheMITbro Formatter — Milestone 21 Acceptance

## Milestone
**Milestone 21 — PDF / HTML Production**

## Objective
Convert the stable M20 question-paper composition output into production PDF and
self-contained HTML formats without changing M20 semantics.

## Required capabilities
- [x] PDF production using ReportLab
- [x] SVG-to-ReportLab vector conversion for M20 pages
- [x] Multi-page PDF output
- [x] Deterministic PDF metadata/output
- [x] Self-contained HTML output
- [x] Inline SVG pages in HTML
- [x] Print CSS for paper-sized output
- [x] Machine-readable M20 manifest retained in HTML
- [x] Dictionary/PaperSpec input support
- [x] Parent directory creation
- [x] M20 regression suite retained

## Boundary
M21 packages the stable M20 rendered-paper representation into PDF and HTML.
It does not redesign question composition, solve questions, generate new diagrams,
or perform large-scale regression testing.

## Acceptance gate
CI must pass:
1. complete regression suite
2. dedicated M21 production tests
3. valid PDF signature/EOF
4. deterministic PDF check
5. self-contained HTML check
6. inline SVG presence
7. M20 validation
8. M21 acceptance summary

A green CI run is required before M22 begins.
