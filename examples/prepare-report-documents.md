# Preparing Report Documents

Assembling a report from multiple source documents is a routine task in many work environments. This guide covers a practical workflow for combining, organizing, and optimizing report PDFs using [PDFProcess](https://pdfprocess.com).

## The Problem

Reports are rarely produced as a single file from the start. A typical report might include:

- A cover page designed in one application
- Body content exported from a word processor
- Charts or data appendices from a spreadsheet
- Supporting documents scanned from paper

Combining these into a single, well-ordered PDF — without installing desktop software or uploading files to a cloud service — is exactly what browser-based PDF tools are built for.

## Workflow

### Step 1: Export Source Documents as PDFs

Convert each section of the report to PDF format. Most applications (word processors, presentation tools, spreadsheet apps) support "Export as PDF" or "Print to PDF."

### Step 2: Merge the Sections

Open the [Merge PDF tool](https://pdfprocess.com/merge-pdf) and add all sections in the intended order:

1. Cover page
2. Table of contents
3. Body sections
4. Appendices
5. Supporting documents

Drag to reorder if needed. Merge the files into a single document.

### Step 3: Review and Trim

If any source PDF contains extra pages (blank pages, draft notes, duplicates), use the [Split PDF tool](https://pdfprocess.com/split-pdf) to extract only the pages you need before merging, or to remove unwanted pages from the merged result.

### Step 4: Compress for Distribution

Reports with embedded images, charts, or scanned appendices can be large. Use the [Compress PDF tool](https://pdfprocess.com/compress-pdf) to reduce file size before sharing. This is particularly useful when the report will be emailed or uploaded to a system with file size limits.

### Step 5: Add Signatures (If Required)

For reports that need approval signatures, use the Sign PDF feature to add a signature directly in the browser. This avoids the print-sign-scan cycle that degrades document quality.

### Step 6: Download the Final Report

The finished document is available for download directly from the browser. No files were uploaded to any server during the entire workflow.

## Example: Quarterly Business Report

| Step | Tool | Action |
|------|------|--------|
| 1 | — | Export cover, body, and financials as PDF |
| 2 | [Merge PDF](https://pdfprocess.com/merge-pdf) | Combine into one document |
| 3 | [Split PDF](https://pdfprocess.com/split-pdf) | Remove draft pages |
| 4 | [Compress PDF](https://pdfprocess.com/compress-pdf) | Optimize for email |
| 5 | Sign PDF | Add director's signature |
| 6 | — | Download final report |

## Tips

- **Consistent formatting.** Export all sections at the same page size (typically A4 or Letter) for a uniform final document.
- **Page numbers.** If individual sections have their own page numbers, consider whether renumbering is needed after merging.
- **Version control.** Keep the original source PDFs alongside the merged report in case you need to revise a single section later.

## Privacy Note

Reports often contain confidential business data — financial results, strategic plans, personnel information. Processing these documents locally in the browser ensures that sensitive content is never transmitted to or stored on external servers. See the [Privacy Model](../docs/privacy-model.md) for details on how this works.

## Related

- [Merge Scanned Documents](merge-scanned-documents.md) — Workflow for combining scanned pages.
- [How Browser PDF Processing Works](../docs/how-browser-pdf-processing-works.md) — Technical details on client-side processing.
