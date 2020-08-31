# Shift_Calculator

### Intro:
For the past year i'm working in shifts, each month i try to recalculate my salary that depends on the number of shifts I worked that month, 
and the most important factor is the time i worked in "shabat time". 
"shabat time" means that from a specific time in friday my hourly wage increase in 150%, and in specific time in saturday my wage is back to regular,
and its important to mention every week the "shabat" entry and exit times are changing. 
I was wasting a lot of time each month to calculate my inncome till i decided i can build a Python code that will do that for me.
I wrote a simple and smart scritp using: BeautifulSoup, requests, openpyxl, datetime, tkinter, prettytable, and pyinstaller modules.
Hope you liked it!

### The scripts:
I create 2 python scripts.
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
