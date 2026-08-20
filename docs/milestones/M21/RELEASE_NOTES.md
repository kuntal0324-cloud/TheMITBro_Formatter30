# Milestone 21 Release Notes

M21 adds production packaging for the stable M20 rendered question paper.

New modules:
- `src/pdf_production.py`
- `src/html_production.py`

PDF uses ReportLab with svglib as the SVG-to-ReportLab conversion bridge.
HTML is self-contained with inline M20 SVG pages and print CSS.

M20 remains the composition source of truth; M21 does not modify PaperSpec
semantics or regenerate diagrams.
