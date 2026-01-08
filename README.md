# HTML Resume (A4) — Joabson de Souza

This repository contains my resume built in **HTML + CSS**, designed to be:

- **ATS-friendly** (clean structure, simple typography, minimal layout noise)
- **Printable in A4** (optimized for exporting to PDF)
- **Easy to customize** (edit content in HTML, styling in CSS)

## What “ATS-friendly” means here

This layout follows common ATS (Applicant Tracking System) best practices:

- Simple, readable HTML (no complex layout tricks required)
- Clear section headings (easy parsing for “Summary”, “Skills”, “Experience”, “Education”)
- Keyword-dense but readable content (optimized for tech job descriptions)
- Links and contact information kept as plain text + standard anchors
- Print rules to avoid awkward breaks (e.g., preventing lists/roles from splitting mid-section)

## Preview

A preview screenshot of the rendered resume is available in the project root:

- `result.png`

## Files

- `index.html` — English version
- `index_ptbr.html` — Portuguese (PT-BR) version
- `styles.css` — Shared stylesheet used by both versions (A4 + print rules)

## How to use

### Open locally
Just open `index.html` (or `index_ptbr.html`) in your browser.

### Export to PDF (A4)
**Chrome (recommended):**
1. Open `index.html`
2. Press `Cmd + P`
3. Set:
   - **Paper size:** A4  
   - **Scale:** 100%  
   - **Margins:** Default (or None)
4. Save as PDF

## Manual page breaks (optional)

You can force a new page by inserting:
```html
<div class="page-break"></div>

The stylesheet includes print rules using:
	•	break-before / page-break-before
	•	break-inside / page-break-inside

to reduce mid-list breaks and keep roles/sections more intact.

Customize
	•	Update content in the HTML files (index.html / index_ptbr.html)
	•	Adjust typography/spacing in styles.css
	•	Keep both HTML files pointing to the same styles.css so the layout stays consistent.

License

Personal use. Feel free to fork and adapt.