# Identifying-Non-EU-European-Countries-Using-Python-Pandas
## Introduction  
This project analyses two datasets — one listing European countries and another listing EU member countries — to determine which European countries are not part of the European Union. It demonstrates a simple but powerful use of **Python**, **Pandas**, and **set operations** to answer a real-world membership question.

## Objectives  
- Import and clean country data from two Excel sheets.  
- Use Python set operations to compare European and EU country lists.  
- Produce a sorted list of European countries that are not EU members.  
- Practice practical data cleaning, manipulation, and comparison workflows.  

## Tools & Libraries  
- **Python 3.x**  
- **Pandas** – for reading Excel files, cleaning data, and manipulating tables.  
- **Python Sets** – for efficient membership and difference operations.  
- **Excel** – as the data source format.  

## Workflow  
1. **Import Data**  
   - Read `Europe` and `EU` sheets from `Europe_and_EU.xlsx` into Pandas DataFrames.  

2. **Clean Data**  
   - Strip leading and trailing whitespace from the `Country` column.  
   - Drop any null or empty country entries.  

3. **Convert to Sets**  
   - Convert the `Country` columns of both DataFrames into Python sets:  
     - `europe_countries` = all European countries.  
     - `eu_countries` = EU member countries.  

4. **Compare Sets**  
   - Check if EU countries are a subset of European countries with `issubset()`.  
   - Use set difference `europe_countries - eu_countries` to find non-EU countries.  

5. **Output Results**  
   - Sort and print the resulting list of non-EU European countries (2018).  

## Skills Demonstrated  
- **Data Import**: Reading multi-sheet Excel files into Pandas.  
- **Data Cleaning**: Standardising string fields and handling missing values.  
- **Data Wrangling**: Extracting unique values from DataFrames.  
- **Set Operations**: Using Python’s built-in set methods (`issubset`, `difference`) to compare groups.  
- **Analytical Thinking**: Breaking a real-world question into a reproducible, code-based workflow.  
- **Result Presentation**: Producing a sorted, human-readable list of findings.  

## Conclusion  
The project shows how combining **Pandas** for tabular data manipulation with simple **Python set operations** can efficiently solve a membership analysis task. This workflow is lightweight, fast, and easily adapted to similar comparison problems in data science.

