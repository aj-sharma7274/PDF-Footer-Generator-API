# PDF-Footer-Generator-API
This Node.js application allows you to add a footer with page numbers to an existing PDF document. The API accepts a base64-encoded PDF and custom footer text to modify the PDF.

Features
Add a footer starting from a specified page in the PDF.
Customize footer text format, e.g., "Page {page} of {pages}".
Supports JSON requests with base64 PDF content.

Requirements
Node.js installed (v14+ recommended)

Install dependencies:
npm install


Request Body Example:
------------------------------------------------URL Start------------------------------------------------------------
http://localhost:3000/add-footer
------------------------------------------------URL End--------------------------------------------------------------
------------------------------------------------Body Start------------------------------------------------------------
{
    "pdfContent": "<base64 encoded PDF content>",
    "footerText": "Page {page} of {pages}"
}
------------------------------------------------Body End------------------------------------------------------------
