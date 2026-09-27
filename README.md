# Unique Info Solution — Certificate Generator

A browser-based certificate generation tool developed by **Harsh** for **Unique Info Solution**.

The application allows users to upload a certificate background/template, add and style certificate fields, manage recipients manually or through CSV, preview certificates, and export individual or bulk certificates as PDF files.

## Project Name

**Unique Info Solution Certificate Generator**

## Developer

**Harsh**  
© 2026 Harsh

## Features

- Upload certificate background/template in JPG or PNG format.
- Drag and drop certificate fields to reposition them.
- Edit certificate text directly from the left-side control panel.
- Show or hide individual fields.
- Customize field:
  - Font
  - Font size
  - Text color
  - Boldness
  - Alignment
  - Text width
- Supported fonts include:
  - Montserrat
  - Playfair Display
  - Dancing Script
  - Great Vibes
  - Crimson Text
  - Arial
  - Georgia
- Recipient management:
  - Add recipients manually.
  - Import recipients from CSV.
  - Delete recipients.
  - Navigate between recipients.
- Automatic certificate number generation for multiple recipients.
- Live certificate preview using HTML Canvas.
- Zoom preview at 50%, 75%, and 100%.
- Download the current certificate as PDF.
- Download the current certificate as PNG.
- Generate and download all certificates as a single bulk PDF.
- Bulk generation progress indicator.
- Sample CSV download.
- Drag-and-drop CSV upload.
- Keyboard navigation using Left/Right arrow keys.
- Toast notifications for successful and failed operations.
- Responsive dark-themed editor interface.

## Default Certificate Fields

The application provides the following configurable fields:

- Recipient Name
- Body Description
- Certificate No.
- Issue Date
- Signature 1
- Signer 1 Title
- Signature 2
- Signer 2 Title

The recipient name is automatically taken from the recipient list when generating certificates.

## CSV Format

The CSV file should contain a `name` column.

Example:

```csv
name
Vijay Upadhyay
Rahul Sharma
Harsh
Priya Singh
Amit Kumar
```

The application also accepts common variations such as `Name`, `naam`, and `Naam`.

## Export

### Individual PDF

Generates a PDF for the currently selected recipient.

Example filename:

```text
certificate_Harsh.pdf
```

### Individual PNG

Generates a PNG image for the currently selected recipient.

Example filename:

```text
certificate_Harsh.png
```

### Bulk PDF

Generates one PDF containing certificates for all recipients.

Example filename:

```text
certificates_bulk_5.pdf
```

## Technology Stack

This project is implemented as a single HTML application using:

- HTML5
- CSS3
- JavaScript
- HTML Canvas API
- jsPDF
- Papa Parse
- Google Fonts

External libraries are loaded through CDN.

## How to Run

No server or build system is required for the current version.

1. Open `certificate-generator.html` in a modern web browser.
2. Upload a certificate background image.
3. Configure the certificate fields.
4. Add recipients manually or upload a CSV file.
5. Adjust field positions and styles.
6. Preview each certificate.
7. Download an individual PDF/PNG or generate the bulk PDF.

## Workflow

```text
Upload Certificate Background
            ↓
Configure Certificate Fields
            ↓
Add Recipients / Upload CSV
            ↓
Position & Style Fields
            ↓
Preview Certificates
            ↓
Export PDF / PNG
            ↓
Bulk PDF Generation
```

## Project Structure

Currently the project is distributed as a standalone HTML file:

```text
certificate-generator.html
README.md
```

The HTML file contains the UI, styling, application state, Canvas rendering logic, recipient management, CSV processing, and export functionality.

## Important Notes

- The certificate background is rendered at its original image dimensions.
- Certificate fields use relative X/Y positions, allowing them to remain aligned with the background.
- The generated PDF uses the certificate image dimensions to determine the PDF page size and orientation.
- Bulk certificates are combined into a single PDF.
- The application runs primarily in the browser; recipient data is processed locally by the page.
- The current implementation does not require a backend server.

## Third-Party Libraries

### jsPDF

Used for PDF generation.

### Papa Parse

Used for parsing recipient CSV files.

### Google Fonts

Used for certificate typography and supported font styles.

## Version

**2026**

## Copyright

© 2026 Harsh — Unique Info Solution
