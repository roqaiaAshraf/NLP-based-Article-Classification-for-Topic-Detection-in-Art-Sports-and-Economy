# Resume Analyzer

This Python script serves as a Resume Analyzer tool, designed to extract contact information and experience sections from resumes uploaded in PDF, DOCX, or TXT formats. The extracted information is then saved to a CSV file named "Contact_information.csv" for further analysis.

## How it Works

**File Reading**: The script reads various file formats (PDF, DOCX, TXT) using the `read_files()` function, which utilizes different libraries (`PyPDF2` for PDF, `docx2txt` for DOCX, and direct decoding for TXT files).

**Contact Information Extraction**: Contact information such as name, email, and phone number is extracted from the resume using regular expressions in the `extract_contact_info()` function. Additionally, the experience section is extracted using a custom regex pattern.

**User Interface**: The tool provides a simple user interface using Streamlit. Users can upload one or multiple resume files for analysis.

**CSV Output**: Extracted contact information and experience sections are stored in a CSV file named "Contact_information.csv". If the file already exists, new entries are appended to it.

## Usage

1. **Upload Resumes**: Click the "Upload your resume files" button and select one or multiple resume files in PDF, DOCX, or TXT formats.

2. **Analysis**: Once files are uploaded, the script automatically extracts contact information and experience sections from each resume.

3. **Output**: Extracted information is displayed on the Streamlit web interface and saved to "Contact_information.csv".

## Requirements

- Python 3.x
- PyPDF2
- pandas
- streamlit
- docx2txt (for DOCX files)

## How to Run

1. Ensure you have Python and required libraries installed.
2. Copy the provided code into a Python script (e.g., `resume_analyzer.py`).
3. Open a terminal or command prompt and navigate to the directory containing the script.
4. Run the script using the command `streamlit run resume_analyzer.py`.
5. Upload resumes for analysis using the provided interface.
