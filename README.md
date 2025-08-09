# Energy Invoices – Electricity Bill Processing (Python)

[🇧🇷 Read in Portuguese](https://github.com/brumor-2/energy_invoices/blob/main/README-pt.md)

This project automates the processing of electricity bills (PDF format) from ENEL for 70 schools.  
The script scans a specific folder for PDF files, renames each file according to the school's name and installation number, extracts the invoice amounts, and generates an Excel spreadsheet with a summary and total value.

---

## Technologies Used
- Python  
- Pandas (Excel manipulation and export)  
- `os`, `re`, `openpyxl` or equivalent libraries for file handling and PDF parsing  

---

## What I Learned
- **Batch file renaming** with a custom mapping based on school and installation number  
- **Data extraction from semi-structured PDF documents**  
- **Data consolidation in Excel**, including total calculations  
- **Real-world Python scripting**, combining file handling, data parsing, and automation  
- **Clear documentation** for reproducibility and adaptation to other contexts  

---

## How to Use
1. Place all PDF bills in the `input_pdfs/` folder.
2. Adjust the mapping in `energy_invoices_base.py` to match your school/installation data.
3. Run:
   ```bash
   python energy_invoices_base.py
The output.xlsx file will be generated with renamed files and a consolidated spreadsheet.

⚠️ Notes
You must adapt the school mapping for your own use — sensitive data is not included in this repository.

The PDF pattern must match the ENEL invoice format for the extraction to work correctly.
