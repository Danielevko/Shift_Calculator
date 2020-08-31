# Shift_Calculator

### Intro:
For the past year i'm working in shifts, each month i try to recalculate my salary that depends on the number of shifts I worked that month, 
and the most important factor is the time i worked in "shabat time". 
"shabat time" means that from a specific time in friday my hourly wage increase in 150%, and in specific time in saturday my wage is back to regular. 
I was wasting a lot of time each month to calculate my inncome till i decided i can build a Python code that will do that for me.
I wrote a simple and smart scritp using: BeautifulSoup, requests, openpyxl, datetime, tkinter, prettytable, and pyinstaller modules.
Hope you liked it!

### The scripts:
I create 2 python scripts.
1) **Import_Shabat_Data_Table** [Link here](https://github.com/Danielevko/Shift_Calculator/blob/master/Import_Shabat_Data_Table.ipynb)
The first one is used to import all the data from the website: "https://calendar.2net.co.il/parasha.aspx".
I import the data using BeautifulSoup and requests modules.

2) **shift_calculator_script** [Link here](https://github.com/Danielevko/Shift_Calculator/blob/master/shift_calculator_script.ipynb)
the second and the main script is doing several things:
first its import the excel file with the shifts data of the current month, and then caluclate the salary according to the "shabat list" we created in the first script.
that means its comparing every shift made in friday or saturday and check the accurate time the wage needs to increase to 150% according to the "shabat list",
that way the salary is more accurate from the most salary software that the accountant are using.

