# Customer results and diagnostic notes

User direction, 16 November 2026:

- A customer opens one result card per document. Preserve page order, printed row order, repeated item rows, and the text-line order inside each item. Do not regroup the document by SKU for this view.
- Export the available data as structured JSON (`bai-ngan.document.v1`) or CSV. Keep literal `text_lines` alongside proposed product code/description. A display label is not an extracted PO number.
- Unknown or unavailable quantities, units, prices and header fields stay `null` in JSON. `null` is not zero and does not certify a printed blank. The current public snapshot contains product text only; financial data are not present.
- Reader names, confidence, alternative readings, source-line pointers and bounding boxes belong in the diagnostic view/export (`bai-ngan.diagnostic.v1`), separate from the customer payload. Keep this evidence available for IT and pipeline development.
- The diagnostic tab is a prototype view switch, not authorization. Real admin-only access will require server-side accounts and permissions; hiding a tab or CSS is not security.
- CSV uses UTF-8 BOM and standard quoted fields. Potential spreadsheet formulas are text-prefixed in CSV; JSON retains the literal text. Neither format grants human verification or production readiness.
- Product-reference images and their match notes remain separate from OCR evidence and do not change the extracted text.

The original parser experiment and its scores are unchanged by this presentation/export layer.
