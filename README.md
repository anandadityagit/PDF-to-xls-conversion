Project Name: PDF to XLS Converter

Description:

This Java program converts a PDF document containing tabular data into a Microsoft Excel (.xls) spreadsheet. It utilizes the Apache PDFBox library for PDF parsing and text extraction, and the Apache POI library for Excel workbook creation and data population.

Features:

Input: Accepts a PDF file as input.
Output: Generates a .xls Excel spreadsheet named "AdityaPDFtoXLS.xls" in the same directory as the Java source code.
Error Handling: Catches exceptions and prints descriptive error messages to the console.
Clarity: Employs meaningful variable names and comments to enhance code readability.

Requirements:

Java Development Kit (JDK) 8 or later
Apache PDFBox library (download from https://pdfbox.apache.org/download.html)
Apache POI library (download from https://poi.apache.org/download.html)

Installation:

Download the Apache PDFBox and Apache POI libraries (JAR files).
Place the JAR files in a directory accessible to your Java project (e.g., project's lib folder).
Configure your IDE (e.g., Eclipse) to include these libraries in the project's build path.

Usage:

Compile the Java source code (pdftoxls.java) using a Java compiler.
Execute the compiled program (pdftoxls) with the path to your PDF file as a command-line argument. Example: java pdftoxls /path/to/your/HolidayList.pdf

Explanation:

Imports: Include necessary libraries for PDF parsing, text extraction, and Excel workbook creation.
main Method:
Validates command-line arguments (expects one PDF file path).
Loads the PDF document using Loader.loadPDF.
Extracts text from the PDF using PDFTextStripper.getText.
Creates a new HSSFWorkbook (Excel 97-2003 format) and a sheet named "Sheet1".
Splits the extracted text into lines and then further splits lines into columns (assuming whitespace-separated values).
Iterates through lines and columns, creating rows and cells in the Excel sheet accordingly.
Writes the workbook to the output file "AdityaPDFtoXLS.xls".
Provides success/error messages to the user.
Exception Handling: Catches IOException during file operations and prints
