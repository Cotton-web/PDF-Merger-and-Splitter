# PDF-Merger-and-Splitter
Program to split a PDF and merge a PDF.
## Requirements
1. Python 3.x
2. PyDF2 library
## Usage
1. Copy the script.
2. Set the paths
   - Enter the path to your input PDF file.
   - Enter the output directory where you want the split PDF files to be saved.
3. Run the script
   python3 name_of_script.py
   
The script will ask you to:

  Enter the page number where you want to split the PDF.

## Script Explanation
**split_pdf Function**
This function takes three arguments:

input_pdf: The path to the input PDF file.
output_dir: The directory where the split PDF files will be saved.
split_page: The page number where the PDF will be split.

The function performs the following steps:

1. Checks if the output directory exists and creates it if it doesn't.
2. Reads the input file.
3. Splits the PDF into two parts based on the specified page number.
4. Saves the two parts as part1.pdf and part2.pdf in the specified output directory.

**merge_pdfs Function**
This function takes two arguments:

input_pdfs: A list of paths to the input PDF files to be merged.
output_pdf: The path where the merged PDF file will be saved.

The function performs the following steps:

1. Creates a PdfWriter object.
2. Iterates over each input PDF file:
3. Opens the PDF file.
4. Reads the PDF file using PdfReader.
5. Adds each page of the PDF to the PdfWriter object.
6. Closes the PDF file.
7. Writes the combined pages to the output PDF file.

**This project is licensed under the MIT License.**
