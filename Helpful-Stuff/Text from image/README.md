# This is using Tesseract-ocr feature

## Pre-Requisite 
1. Python 3.5 or above ~ pip install opencv
2. Tesseract-ocr :
[Source1](https://github.com/tesseract-ocr/tesseract)
[Source2](https://tesseract-ocr.github.io/tessdoc/Home.html)
[Download](https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-v5.0.0-alpha.20200328.exe)

## Simple Code Execution :
```
import cv2
import pytesseract
pytesseract.pytesseract.tesseract_cmd = r'C:\\Program Files\\Tesseract-OCR\\tesseract.exe' //{Path to tesseract.exe}
img = cv2.imread('<insert image filename>') //include path if its in a different location
text = pytesseract.image_to_string(img)
print(text)
```
**END**
