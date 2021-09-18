# PDF2CSV - Converter

Convert pdf timetable to csv

# Question on StackOverflow
https://stackoverflow.com/questions/69232521/convert-a-tabled-pdf-data-into-a-text-or-any-other-readable-format-file-using
               

## How it Works
                
It works in 3 steps

**Step 1** - Conversion of PDF to PNG

**Step 2** - Conversion of PNG to TXT

**Step 3** - Formatting of TXT to CSV




## Installation
               

1) You will need python 3 installed, latest version will do.
2) Download [poppler](https://blog.alivate.com.au/poppler-windows/ "poppler") for your operating system.
3) Download [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract/wiki "Tesseract-OCR") for your system and install it. 
4) In cmd/terminal,
       
    `pip install pytesseract`  
5) Install pdf2image and pillow by 

   `pip install pdf2image`
    `pip install pillow`
5) Clone or download the files in this repo and extract them.
6) Done!

## How to use
               

1) Open the `config.ini` file in your favourite text editor and enter in it, the path of 'poppler' bin directory and 'Tesseract' and save the file.
2) In cmd/terminal/Power shell enter
       
	   python pdf2csv.py -i filetoconvert.pdf
     to run for whole file
       
	   python pdf2csv.py -i filetoconvert.pdf -fp 1 -lp 5
     to run for 5 pages of the file
3) DONE!

Tip - If you want to convert a file in different folder, in cmd, put full address, eg.

	   python pdf2.csv.py -i "C:\Users\USERNAME\someRandomFolder\samplefile.pdf"

It is advised to put the address in double inverted commas because it avoids error due to folder with spaces in their name.

PS - type `python pdf2csv.py -h` to see all available arguements in command line.

## Modules involved

- PIL or pillow
- csv
- pytesseract
- os
- pdf2image
- argeparse
- configparser
- pathlib

# Special Thanks
See original code: https://github.com/SahilChoudhary22/pdf2csv-converter
Follow: https://github.com/SahilChoudhary22
