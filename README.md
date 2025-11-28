# Document Highlighter Tool
This project highlights a given search text inside **PDF**, **Word**, **Excel**, and **Image** files by drawing **red bounding boxes** around every match.  
It creates a new output file while keeping the original file unchanged.

---

## Features
- Works on **PDF (.pdf)**  
- Works on **Images (.png, .jpg, .jpeg)**  
- Works on **Word (.docx)** and **Excel (.xlsx)** by converting them to PDF  
- Uses **PyMuPDF** to find text in PDFs  
- Uses **Tesseract OCR** to detect and highlight text in images  
- Highlights text with a **red rectangle**  
- Outputs a _new highlighted file_ (`*_highlighted.pdf` or `*_highlighted.png`)

---

## Installation Instructions

### Recommended: Run in Google Colab  
1. Open **Google Colab**: https://colab.research.google.com  
2. Create a new notebook  
3. Run the following installation cell:

```bash
!pip install pymupdf pillow pytesseract pdf2image pandas
!apt-get update -y
!apt-get install -y tesseract-ocr poppler-utils libreoffice
