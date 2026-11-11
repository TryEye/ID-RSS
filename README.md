# ID-RSS

ID-RSS is a Flask-based document intelligence system for extracting structured details from large batches of Word documents. It helps organize messy student or employee records into a clean, exportable spreadsheet without manually opening each file.

## What this project does

- Reads `.docx` and `.txt` files from a chosen folder
- Extracts fields using pattern-based parsing and validation
- Ranks each result by confidence score
- Displays extracted values in a browser-based interface
- Exports the cleaned data to Excel for reporting or uploading

## Main features

- Batch processing for multiple documents
- Confidence scoring for partial or failed extractions
- Dark-mode web UI for review and validation
- Excel export with styled output
- Demo dataset included for testing and presentation

## Project structure

- `App.py` — Flask application and API routes
- `Extractor.py` — document parsing and field extraction logic
- `Exporter.py` — Excel generation and formatting
- `Templates/index.html` — frontend interface
- `demo_files/` — sample input documents used for testing
- `output.xlsx` — generated export file example
- `requirements.txt` — Python dependencies

## Requirements

- Python 3.10+
- pip

## Setup

```bash
pip install -r requirements.txt
```

## Run the app

```bash
python App.py
```

Then open:

```text
http://localhost:5000
```

## Typical workflow

1. Upload or point to a folder with `.docx` files.
2. Select the fields to extract.
3. Review confidence scores and found values.
4. Export the final dataset to Excel.

## Demo files

The repository includes sample files in `demo_files/` so the app can be tested immediately without additional setup.

## License

This project is provided for educational and demonstration purposes.

