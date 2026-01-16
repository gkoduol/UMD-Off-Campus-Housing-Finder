# UMD Off-Campus Housing Finder
**About the Poject**
A Python-based housing finder application designed specifically for University of Maryland students to search and analyze off-campus apartment options.
**Project Description**
This project helps UMD students find off-campus housing by processing apartment data and allowing users to filter based on their preferences. The application reads housing data from CSV files and provides detailed insights about available apartments near campus. 

**Features**
Data Processing: Reads and processes housing data from a CSV file.
- Apartment Details: Displays key information, including:
- Property name
- Number of bedrooms
- Number of bathrooms
- Monthly rent per person
- Square footage
- Distance from campus (calculated from the STAMP Student Union)

**Accessing the Repository**
You can view the project files and code directly on GitHub:
https://github.com/kmach1/INST326-Final-Project
No need to clone the repository unless you want to run the project locally.

**Usage**
- Command-Line / gui interface
The program is run from the command line. It processes an input file containing apartment data (given), applies filters specified by the user, and saves the cleaned data to a CSV file.

(Example Command to start gui)
"""python gui.py""

Arguments on command line:
None, just run the gui.py file.

**GUI**
![image](https://github.com/user-attachments/assets/6abf6604-3fe7-4af6-94a7-2e6ad6de8d56)

Once the application boots up, it will load the data
  - If booted correctly, the message: "Housing data sucessfully loaded" will apear

![image](https://github.com/user-attachments/assets/741586ed-223a-4bd0-b689-87323b2291f0)
    
The user then specifies the following:
  - Bedroom minimum / maximum (1-5)
  - Bathroom minimum / maximum (1-5)
  - Price minimum / maximum (0-[no limit])
  - Distance minimum / maximum (0-[no limit])
  - Prioritization, aka. what the results filter MUST include*
      *If something is not prioritized then there are alters to the user's specifications to           include more housing data. (how much each category is altered is described in the gui)

![image](https://github.com/user-attachments/assets/e9643936-cf3f-4ce1-a699-a6e58aed9c47)

Example inputs / outputs (also in the gui)

Example 1: input/output [with all priorities] selected
  Bedrooms: 2-3
  Bathrooms: 2-3
  Price: $500 - $1500
  Distance: 1-4 miles

Results:
  1 | Tempo: 2 beds, 2 baths, $1429, 825 sqft, 1.0 miles
  2 | Tempo: 3 beds, 3 baths, $1425, 839 sqft, 1.0 miles

Example 2: input/output [with NOT all priorities selected] 
  Bedrooms: 2-3
  Bathrooms: 2-3
  Price: $500 - $1500
  Distance: 1-4 miles | Priority box not checked

Results:
  1 | University View: 2 beds, 2 baths, $1249, unknwon sqft, 0.8 miles 
  2 | Tempo: 2 beds, 2 baths, $1429, 825 sqft, 1.0 miles
  3 | Tempo: 3 beds, 3 baths, $1425, 839 sqft, 1.0 miles
  4 | The Standard: 2 beds, 2 baths, $1429, 718 sqft, 0.9 miles
  5 | The Standard: 3 beds, 3 baths, $1399, 1109 sqft, 0.9 miles

After the user inputs the specifications the results will display after selecting "Apply Filters" within the "Results" pannel:
![image](https://github.com/user-attachments/assets/7e94d7da-6c4a-40d6-93c2-33f0a3db7f8e)

![image](https://github.com/user-attachments/assets/5ecd231f-f629-41a8-9ad8-79daf50e51df)


Contributions 
Karalyn Mach, Genevieve Koduol, Theodore Rose, Sarah Bamba

Distributed under the MIT License. See LICENSE.txt for more information.
MIT License




