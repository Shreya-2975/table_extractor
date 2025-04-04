# 📄 Table Extractor from PDFs to Excel 🚀

## 📌 Overview
Easily detect and extract tables from **system-generated PDFs** without using **Tabula, Camelot, or image conversion techniques**! This tool efficiently processes tables with and without borders, including irregularly shaped tables, and stores them in an Excel sheet.

## 🎥 Demo Video
[Demo Video Link](https://drive.google.com/drive/folders/1GnpsZJ5CiWdG9h1Ng8BEZv_FQmT-xQ1q?hl=en&q=sharedwith:public%20parent:1GnpsZJ5CiWdG9h1Ng8BEZv_FQmT-xQ1q)

## ✨ Features
- ✅ **Smart Table Recognition** – Identifies table structures with precision.
- ✅ **Works with Any Layout** – Supports tables with or without visible borders.
- ✅ **Adaptive to Complex Tables** – Handles irregularly shaped and multi-line tables.
- ✅ **Automated Data Cleaning** – Removes duplicates and unnecessary spaces.
- ✅ **Multi-Page Support** – Extracts tables from all pages in a PDF.
- ✅ **Bulk Processing** – Processes multiple PDFs in a folder automatically.
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
- 🔹 **Load the PDF** – Uses `PyMuPDF (fitz)` to open and analyze the document.
- 🔹 **Extract Words & Positions** – Retrieves words along with their positional coordinates.
- 🔹 **Detect Table Structure** – Identifies table rows and columns by analyzing word alignment and spacing.
- 🔹 **Process & Clean Data** – Removes empty values, trims spaces, and eliminates duplicate headers.
- 🔹 **Export to Excel** – Saves each detected table into a structured Excel sheet.
- 🔹 **Batch Processing** – Automatically processes multiple PDFs from a given folder.


## ⚠️ Limitations
- 🚫 May not work well with **handwritten or highly complex scanned PDFs**.
- 🚫 **Very irregular tables** might need **manual adjustments**.

## 🌍 GitHub Workflow
1. **Initialize a Git repository**:
   ```sh
   git init
   ```
2. **Add files to the repository**:
   ```sh
   git add .
   ```
3. **Commit changes**:
   ```sh
   git commit -m "Initial commit - Added PDF table extractor script"
   ```
4. **Create a new repository on GitHub** and copy the repository URL.

5. **Push code to GitHub**:
   ```sh
   git push -u origin main
   ```
6. **Update repository**:
   - If  make changes, repeat steps **2-6** to push updates.







