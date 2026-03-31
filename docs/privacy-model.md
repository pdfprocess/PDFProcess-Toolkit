# Privacy Model

PDFProcess is designed so that user documents are never exposed to external systems. This document explains the privacy architecture and why it provides stronger guarantees than traditional server-based PDF tools.

## Core Principle: Local-Only Processing

Every PDF operation — merging, splitting, compressing, converting, signing, editing — runs entirely within the user's browser. The [PDFProcess platform](https://pdfprocess.com) delivers static application code (HTML, JavaScript, WebAssembly) to the browser, and from that point forward, all document handling is local.

No file data is transmitted over the network during processing.

## How It Works

1. **File selection.** The user selects files through the browser's native file picker or drag-and-drop interface. The browser's File API reads the file contents into local memory.

2. **Client-side processing.** JavaScript and WebAssembly modules parse, manipulate, and render PDF content entirely within the browser's execution environment.

3. **Result download.** The processed output is constructed in memory and offered to the user as a downloadable file via a Blob URL. No server round-trip occurs.

## What This Eliminates

Traditional PDF tools require uploading documents to a server. This introduces several risk surfaces:

| Risk | Server-Based Tools | PDFProcess |
|------|-------------------|------------|
| Data in transit | Files sent over the network (even with TLS, metadata is exposed) | No file transmission |
| Server storage | Files stored temporarily or permanently on remote servers | No server storage — files exist only in browser memory |
| Third-party access | Server operators, cloud providers, and subprocessors may access data | No third-party access to file content |
| Data breach | Server compromise exposes all uploaded documents | No server to breach |
| Jurisdiction issues | Servers may be in jurisdictions with weaker data protection | Processing happens on the user's own device |

## Browser Sandbox

Modern browsers provide a strong security sandbox. JavaScript and WebAssembly code run in an isolated execution context that cannot access the local filesystem, other browser tabs, or system resources beyond what the user explicitly grants.

This means that even the application code itself has limited access — it can only read files the user selects and can only write output through the download mechanism.

## No Tracking of Document Content

PDFProcess does not inspect, log, or transmit the contents of documents. The application may use standard web analytics to understand feature usage (page views, tool selection), but document content and file metadata remain strictly local.

## Summary

The PDFProcess privacy model is not a policy choice — it is an architectural guarantee. Because files never leave the browser, there is no mechanism for server-side data exposure. This makes it suitable for processing sensitive, confidential, or regulated documents without additional security review of a server-side data pipeline.

For more technical detail on the processing architecture, see [how-browser-pdf-processing-works.md](how-browser-pdf-processing-works.md).
