# Extracting-and-Processing-Timetable-Data-from-Excel

1. Introduction

This Python script extracts timetable data from an Excel file and processes it into a structured format. The Excel file contains multiple sheets, each representing a different day. The script reads data from each sheet starting from a specified row and organizes it into a DataFrame for easy analysis and manipulation.

2. Features

Excel Data Extraction: Reads multiple sheets from an Excel file and processes the timetable data.
Data Cleaning: Extracts relevant information and handles various data formats.
Structured Output: Organizes the extracted data into a Pandas DataFrame.

3. System Requirements

Python 3.6 or later

Pandas library

openpyxl library

A terminal or command-line interface

4. Installation

Install Required Libraries:

Ensure you have Pandas and openpyxl installed. You can install them using pip:

bash

Copy code

pip install pandas openpyxl

Clone the Repository: Clone this repository to your local machine using:



bash


Copy code
git clone <repository_url>

Navigate to the Directory:




bash

Copy code

cd <repository_directory>
Run the Script:



bash

Copy code

python extract_timetable.py

Replace <repository_url> and <repository_directory> with the actual URL and directory name.



5. Usage
Prepare the Excel File: Ensure your Excel file TimeTable.xlsx is in the same directory as your script.



Run the Script: Execute the script to extract and print the timetable data.



6. Code Overview

Import Libraries

python

Copy code
import pandas as pd

Import Pandas for data manipulation and openpyxl for reading Excel files.



Load the Excel File

python

Copy code
file = pd.ExcelFile("TimeTable.xlsx", engine='openpyxl')

Load the Excel file using Pandas.

Extract Data from Each Sheet

python



Create Final DataFrame

python
Copy code

final_df = pd.DataFrame(all_data_dicts)

Combine all extracted data into a single DataFrame.

Print the Resulting DataFrame

python

Copy code

print(final_df)

Print the final DataFrame for review.

7. Examples

Example Output
mathematica

Copy code
    Room       Day                Course Section   Type        Time
0  Room1  Monday   Data Structures    101 Theory    9:00-10:00

1  Room1  Monday     Linear Algebra    102 Theory  10:00-11:00

2  Room2  Tuesday         Calculus     103 Theory    9:00-10:00

3  Room2  Tuesday        Chemistry     104 Theory  10:00-11:00

Note: Replace actual values with relevant data from your timetable.



8. Author
This script was created by [Your Name]. For any questions or support, please contact bilal.aleem2406@gmail.com or 03333332460


