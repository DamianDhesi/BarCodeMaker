# BarCodeMaker

## Usage notes

* In order to utilze the barcode maker follow the steps below
  - Place the barcode maker executable in its own folder
  - Place the font fitle (.ttf) in the same folder as it will not work otherwise
  - format the desired barcode numbers in the exact same way as /test/Book1.xlsx
  - Run the executable to generate a BardCode folder with all the barcodes in .png format
    - works only on windows devices
 * Support for the the generation of barcodes as .zpl files was attempted but never completed

 ## Code Design

 This program is by no means well designed as I was given a short time frame and was only able to work on the project for roughly 5 hours with no prior knowledge on barcode generation. However, it does demonstrate my ability to quickly learn python barcode libraries and bug test enough to create a minimum viable product in a restrictive time frame.

 ## Purpose

 I was contacted by a realtive working in operations at Republic National Distribution Company (RNDC) that their barcode generater failed to correctly format the barcodes for the inventory at their warehouse. They requested if I would volunteer to create a program to generate the barcodes in the correct format and size by the end of the day. While I could have easily denied the request due to my lack of experience in generating barcodes and the short time frame given, I decided to accept the request as a way to challenge myself.

After spending roughly 5 hours learning barcode libraries for python, coding, and bug testing I was able to create a minimum viable product that generated the barcodes in the correct format and size. I also attempted to create a program to convert the generated .png files of the barcodes and convert them to .zpl format so that they could be more easily printed from a zebra barcode printer (BCtoZPL.py) . However, the conversion was not necessary as the BarCodeMaker.exe was sufficent in allowing the IT team at the warehouse to generate barcodes of the correct size and format.

## Lessons Learned

* Gained expereince in quickly learning new libraries
* Developed skills in identifying the needs and wants of a program user
* Learned how to create a minimum viable product in a short time frame

## Utilized Libraries 

* [Openpyxl](https://pypi.org/project/openpyxl/): used to get the barcode numbers from the xecl file
* [python-barcode](https://pypi.org/project/python-barcode/): used to generate the barcodes
* [PyInstaller](https://pypi.org/project/pyinstaller/): used to compile the code into an executable
