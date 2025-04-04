# 📄 Table Extractor from PDFs to Excel 🚀

## 📌 Overview
Easily detect and extract tables from **system-generated PDFs** without using **Tabula, Camelot, or image conversion techniques**! This tool efficiently processes tables with and without borders, including irregularly shaped tables, and stores them in an Excel sheet.

## ✨ Features
- ✅ **Smart Table Recognition** – Identifies table structures with precision.
- ✅ **Works with Any Layout** – Supports tables with or without visible borders.
- ✅ **Adaptive to Complex Tables** – Handles irregularly shaped and multi-line tables.
- ✅ **Multi-Page Support** – Extracts tables from all pages in a PDF.
- ✅ **Excel Export** – Saves structured table data in a clean Excel sheet.

## ⚡ Installation
Ensure Python is installed on your system, then install the required dependencies:

```bash
pip install pandas pdfplumber openpyxl
```

## 🛠 Usage
Run the script with the **PDF file path** and desired **Excel output filename**:

```bash
python extract_tables.py input.pdf output.xlsx
```

### 📌 Example:
```bash
python extract_tables.py sample.pdf extracted_tables.xlsx
```

## 🔍 How It Works
-1️⃣ **Loads the PDF** – Uses `PyMuPDF (fitz)` to open and analyze the document structure.
-2️⃣ **Extracts Words & Coordinates** – Retrieves words with their positional data.
-3️⃣ **Identifies Table Rows** – Groups words based on alignment and spacing.
-4️⃣ **Refines Data** – Cleans empty values, trims extra spaces, and removes duplicate headers.
-5️⃣ **Exports to Excel** – Saves each table in a separate sheet for better organization.
-6️⃣ **Processes Multiple PDFs** – Automatically extracts tables from all PDFs in a specified folder.

## ⚠️ Limitations
- 🚫 May not work well with **handwritten or highly complex scanned PDFs**.
- 🚫 **Very irregular tables** might need **manual adjustments**.






