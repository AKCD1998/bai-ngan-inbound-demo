# MOCK-only audit

- All 3 document objects rebuilt from synthetic constants, not redacted original rows.
- 3 newly generated mock PDFs / 11 pages; no original PDF copied.
- 75 synthetic rows, all quantities/prices/totals fictional.
- 8 original geometric SVG illustrations generated for fictional products.
- UI, JSON, CSV and diagnostics use the mock dataset.
- Original company/product/part/document IDs and source SHA denylist: zero matches in output text or extracted PDF text.
- No original data files, original assets, email IDs or recovered git history copied.
- Deployment uses a fast-forward commit on existing public main. Existing public history is preserved; no private checkpoint ancestor is included.
- Node data/render functions and mock-DOM navigation tests pass. Browser visual/interaction test not verified.
- Public deployment explicitly approved for this fictional mock only.
