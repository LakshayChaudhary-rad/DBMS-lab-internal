import pypandoc, os

content = """# DBMS Lab Internal

A collection of Database Management Systems (DBMS) lab sheets for quick reference, practice, and revision.

## Repository Contents

This repository currently contains the following lab-sheet PDFs:

- `DBMS_Labsheet_1 (1).pdf`
- `DBMS_Labsheet_2 (1).pdf`
- `DBMS_Labsheet_3 (1).pdf`
- `DBMS_Labsheet_4 (1).pdf`
- `DBMS_Labsheet_5 (1).pdf`

## How to Use

1. Open the lab sheet you need from the repository.
2. View or download the PDF.
3. Use the sheets to complete the corresponding DBMS lab exercises and revise the concepts covered in class.

## Purpose

This repository keeps the DBMS lab materials organized in one place so they are easy to access and review.

## Notes

- The repository contains the PDF files currently uploaded.
- Add new lab sheets to this repository as they become available.
- Check your course instructions for submission requirements and deadlines.

---

Maintained by **LakshayChaudhary-rad**.
"""
output = "/mnt/data/README.md"
pypandoc.convert_text(content, "md", format="md", outputfile=output, extra_args=["--standalone"])
print(f"Created: {output}")
