# File Format Text Extraction

This repository provides Python code examples for extracting text from different file formats such as PDF, DOC, HTML, XML, JSON, and CSV using various libraries.

## Supported File Formats

1. **PDF**
2. **DOC**
3. **HTML**
4. **XML**
5. **JSON**
6. **CSV**

## Libraries and Approaches

### PDF to Text Conversion

#### PyPDF2

- **Approach:**
  - Extracts text from PDF files using `PyPDF2`.
  - Methods:
    - `reader.pages[page_number]`
    - `reader.numPages`
    - `reader.metadata`
    - Rotate PDF pages using `writer.getPage(pageNumber)`

#### PyMuPDF (fitz)

- **Approach:**
  - Faster and supports multiple file formats.
  - Methods:
    - `Document.page_count`: Retrieves the number of pages.
    - `Document.metadata`: Extracts metadata.
    - `Document.get_toc()`: Retrieves the table of contents.
    - `Document.load_page()`: Loads and reads a specific page.

### DOC to Text Conversion

#### Spire.Doc

- **Approach:**
  - Extracts specific paragraphs and sections from DOC files.

#### Docx2txt

- **Approach:**
  - Simple extraction using `docx2txt.process`.

### HTML to Text Conversion

- **Approach:**
  - Uses `html2text` and `BeautifulSoup` for HTML parsing.

### XML to Text Conversion

- **Approach:**
  - Utilizes `ElementTree` and `BeautifulSoup` for XML parsing.

### JSON to Text Conversion

- **Approach:**
  - Uses `pandas` and native JSON libraries for conversion.

### CSV to Text Extraction

- **Approach:**
  - Converts CSV to HTML using `pandas`.
  - Utilizes `PDFkit` Python API to convert HTML to PDF.

