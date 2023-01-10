# Salary Shift Calculator
### Intro:
For the past year I’ve been working in shifts. Every month I found myself trying to calculate my upcoming salary depending on the number of shifts I did, while taking in account regular shifts (Sunday to Thursday) and weekend shifts (Friday to Saturday).
The crucial factor of this calculating program was the weekend shifts, called “Sabbath Time”, that differ in their rate and given salary, while the concept is pretty easy to catch. From the commencement of the Sabbath, the salary rate goes up to 150% its’ normal hourly wage, and when the Sabbath ends it goes back to its’ normal rate. 
The main struggle was to constantly check the specific times of when the Sabbath starts and when it ends, in order to calculate the exact anticipated salary.
I used to waist a lot of times trying to calculate my income by myself, until I realized I can build my own Python program that will do that for me.
Hence, I wrote a smart and simple script using numerous Python libraries:  BeautifulSoup, requests, openpyxl, datetime, tkinter, prettytable, and pyinstaller modules. Hope you like it!

### The scripts:

I created 2 python scripts:
1) **Import_Shabat_Data_Table** [Link here](https://github.com/Danielevko/Shift_Calculator/blob/master/Import_Shabat_Data_Table.ipynb)

This script is used to import all the data from the website "https://calendar.2net.co.il/parasha.aspx" using the BeautifulSoup and requests modules.

2) **shift_calculator_script** [Link here](https://github.com/Danielevko/Shift_Calculator/blob/master/shift_calculator_script.ipynb)

The second and main script is doing several things: 
First of all, it imports the Excel file that contains the shifts data of the current month. Secondly, it calculates the salary according to the ‘Sabbath list’ we created in the first script. The code checks every shift (which is represented by a single Excel cell) from the Excel file. If the shift was done on Friday or Saturday, it compares the shift date with the ‘Sabbath list’. In case the dates match, we can extract the exact entry and exit times according to the website, and then calculate the time our wage goes up to Sabbath rate, which is 150%. That way our salary is calculated more accurately than most salary software that accountants are still using today.

### Usage
Run the Import_Shabat_Data_Table script to import the data.
Run the shift_calculator_script script and provide the path to the excel file with your shift data.
The program will then output the calculated salary.

### Note
before running the script make sure that all the necessary library are installed, otherwise install the library by running pip install <library name>
Contributions
If you have any suggestions or find any bugs please open an issue or create a pull request.

Thank you for using my program, I hope it helps make calculating your salary a little bit easier!
