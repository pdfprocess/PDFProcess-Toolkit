# Merging Scanned Documents

A common workflow when digitizing paper documents is scanning pages individually and then combining them into a single PDF. This guide walks through how to accomplish that using [PDFProcess](https://pdfprocess.com).

## The Problem

Scanners — particularly mobile scanning apps and basic flatbed scanners — often produce one PDF per page or one image per scan. A 10-page document might result in 10 separate files. Combining these into a single, ordered PDF is a frequent need for:

- Archiving paper records
- Submitting multi-page forms
- Organizing receipts or invoices
- Creating a single file from a batch scan

## Workflow

### Step 1: Gather Your Scanned Files

Collect all scanned pages on your device. Supported formats include individual PDFs and images. Rename files with a numeric prefix if your scanner does not produce them in order (e.g., `01-cover.pdf`, `02-page1.pdf`).

### Step 2: Open the Merge Tool

Navigate to the [Merge PDF tool](https://pdfprocess.com/merge-pdf) in your browser.

### Step 3: Add Files

Select all scanned files using the file picker or drag and drop them onto the page. The tool will display a preview of each file in the order they were added.

### Step 4: Arrange Page Order

Reorder files by dragging them into the correct sequence. This is especially useful when scanned pages were not captured in order.

### Step 5: Merge and Download

Click the merge button. The tool combines all files into a single PDF directly in your browser. The merged file is then available to download.

No files are uploaded to any server during this process. Everything happens locally on your device.

## Tips

- **File size.** Scanned documents tend to be large due to high-resolution images. If the merged file is too big, use the [Compress PDF tool](https://pdfprocess.com/compress-pdf) to reduce its size.
- **Page orientation.** If some scanned pages are rotated, you can fix orientation before or after merging using the Edit PDF feature.
- **Batch scanning.** Some scanners can produce a multi-page PDF directly. If yours does, you may only need to merge a few multi-page files rather than many single-page files.

## Privacy Note

Because PDFProcess processes files locally in the browser, scanned documents — which often contain sensitive personal information like IDs, medical records, or financial statements — never leave your device. This makes it a practical choice for handling confidential scans without worrying about data exposure.

## Related

- [Prepare Report Documents](prepare-report-documents.md) — Another common workflow for combining documents.
- [Privacy Model](../docs/privacy-model.md) — How local processing protects your data.
