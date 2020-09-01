# Shift_Calculator

### Intro:
For the past year I’ve been working in shifts. Every month I found myself trying to calculate my upcoming salary depending on the number of shifts I did, while taking in account regular shifts (Sunday to Thursday) and weekend shifts (Friday to Saturday).
The crucial factor of this calculating program was the weekend shifts, called “Sabbath Time”, that differ in their rate and given salary, while the concept is pretty easy to catch. From the commencement of the Sabbath, the salary rate goes up to 150% its’ normal hourly wage, and when the Sabbath ends it goes back to its’ normal rate. 
The main struggle was to constantly check the specific times of when the Sabbath starts and when it ends, in order to calculate the exact anticipated salary.
I used to waist a lot of times trying to calculate my income by myself, until I realized I can build my own Python program that will do that for me.
Hence, I wrote a smart and simple script using numerous Python libraries:  BeautifulSoup, requests, openpyxl, datetime, tkinter, prettytable, and pyinstaller modules. Hope you like it!

### The scripts:
I created 2 python scripts:
1) **Import_Shabat_Data_Table** [Link here](https://github.com/Danielevko/Shift_Calculator/blob/master/Import_Shabat_Data_Table.ipynb)

The first one is used to import all the data from the website: "https://calendar.2net.co.il/parasha.aspx".
I import the data using BeautifulSoup and requests modules.

2) **shift_calculator_script** [Link here](https://github.com/Danielevko/Shift_Calculator/blob/master/shift_calculator_script.ipynb)

The second and the main script is doing several things:
first its to import the excel file that contains the shifts data of the current month, 
and then caluclate the salary according to the "shabat list" we created in the first script.
the code check every shift (an excel cell) from the excel file, if the shift was done in friday or saturday its comparing the shift date with the "shabat list", 
after the dates are match, we can extract the exact entry and exit times according to the website, 
and then calculate the time our wage needs to be increased by 150%.
that way our salary is more accurate then most salary software, that accountants are still using today.
